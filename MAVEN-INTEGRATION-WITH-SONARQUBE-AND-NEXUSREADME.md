INTERGRATING MAVEN WITH SONAQUBE AND NEXUS
-

make sure you are in your project directory in the maven
server before intergrating with other tools;
e.g 
    sonarqube and nexus

for you to intergrate maven with sonarqube; you vi into
the pom.xml file of the project, search for the properties 
tag and enter the sonarqube server's ipaddress, to do that;

             vi pom.xml # make sure you are in the project
                          directory


when you run the command vi /vim pom.xml, you will find a tag
like this below, change the sonar.host.url ipadress(e.g 18.209.180.44)
to that of your sonarqube server 

<properties>
                <jdk.version>1.8</jdk.version>
                <spring.version>5.1.2.RELEASE</spring.version>
                <junit.version>4.11</junit.version>
                <log4j.version>1.2.17</log4j.version>
                <sonar.host.url>http://18.209.180.44:9000/</sonar.host.url>
                <sonar.login>admin</sonar.login>
                <sonar.password>admin</sonar.password>
                <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
                <project.reporting.outputEncoding>UTF-8</project.reporting.outputEncoding>
        </properties>

After doing that, save and quit with; :wq!

FOR NEXUS
-

Access your nexus server on the browser,
you can do this by entering your nexus server's 
ipaddress and the nexus port number (8081)
on the browser,
   e.g 
        https://18.204.7.129:8081

when you successfully access the nexus server on the browser,
login with the default username and poassword;

           username  =  admin
           password  =  admin123

After logged in,
  click on the server administration and configuration botton
  which has sign like that of the setting sign, it will take 
  you to a page as below

-----------   ----------------  ------------  -----------------
blob stores   cleanup policies  Repositories  Content Selectors
-----------   ----------------  ------------  -----------------  

- Click on Repositories
- Take create repository
- Select, maven2 (host)
- Enter the repo-name where you see name e.g toyotarelease
- Click on version policy and select, release
- Allow layout policy to be strict
- click on deployment policy and select, allow redeploy
- Click on create repositoy to create the maven-remote-repo

* do same when creating for snapshot repo

After creating the repositories, click on copy on each of the created repositories and copy the repo url(s) .

Go to your maven server,
stwich to your project directory
vi into the pom.xml file
  
          vi /vim pom.xml

make sure you are in you project directory
search for the distributionmanagement tag,
you will see a tag as below  



<distributionManagement>
            <repository>
              <id>nexus</id>
              <name>Landmark Technologies Releases Nexus Repository</name>
              <url>http://18.204.7.129:8081/repository/releases/</url>
            </repository>

            <snapshotRepository>
              <id>nexus</id>
              <name>Landmark Technologies Snapshot Nexus Repository </name>
              <url>http://18.204.7.129:8081/repository/snapshots/</url>
            </snapshotRepository>

replace the release url below in the tag with the one you
created

http://18.204.7.129:8081/repository/releases/

Do same for that of the snapshot

After replacing the two urls, save and quit; :wq!

Now set the nexus login credentials in the maven server
To do this, you vi into the below file by running;

               sudo vi /vim /opt/maven/conf/settings.xml

In this file, check for the server's tag
You will see a tag as below

<servers>
    <!-- server
     | Specifies the authentication information to use when connecting to a particular server, identified by
     | a unique name within the system (referred to by the 'id' attribute below).
     |
     | NOTE: You should either specify username/password OR privateKey/passphrase, since these pairings are
     |       used together.
     |
    <server>
      <id>deploymentRepo</id>
      <username>repouser</username>
      <password>repopwd</password>
    </server>
    -->

    <!-- Another sample, using keys to authenticate.
    <server>
      <id>siteServer</id>
      <privateKey>/path/to/private/key</privateKey>
      <passphrase>optional; leave empty if not used.</passphrase>
    </server>
    -->
  </servers>

Copy the below tag from it and modify the following
login credentials ;

        - deploymentrepo
        - repouser
        - repopwd

with that of you nexus server   
e.g
    copy the tag you see below

<server>
      <id>deploymentRepo</id>
      <username>repouser</username>
      <password>repopwd</password>
    </server>

and replace the login credentials with that of your nexus server
i.e
    
 <server>
      <id>nexus</id>
      <username>admin</username>
      <password>admin123</password>
    </server> 

NOTE;
-
     you can change this credentials for you nexus server
     so make sure to enter valid credentials;

Here i used the default credentials

After doing that, copy the tag and paste it just before the 
end of the server's tag where you see ;

          -->
         </server>

In between; paste the tag there

make sure not to mess up the file

After modifying the file by pasting the tag, save and quit; :wq! 
