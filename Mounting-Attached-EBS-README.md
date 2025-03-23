**Mounting EBS Volume**

To list block
             
              lsblk

To check memory              
             
              df -h

Check if there is any file system in the instance

          sudo file -s /dev/xvdf

Use the below command to get information about all the 
of the devices attached to the instance.

         sudo lsblk -f

Make the file system for the EBS volume that you want
to mount.

          sudo mkfs -t xfs /dev/xvdf

If you get an error that mkfs.xfs is not found, use the
following command to install the XFS tools and then repeat teh previous command.

          sudo yum install xfsprogs

Use mkdir command to create a mount point directory for the volume. The mount point ois where the volume is located in the file treee and where you read and write files to, after you mount teh volume.

           sudo mkdir /data
           
           sudo mkdir /app

Mount the volume or partition at the mount point directory you created in the previous step. If the volume has no partition, use the following command specify the name to mount the entire volume.

           sudo mount /dev/xvdf /data

If the volume has partition, use the following command and specify the partition name to mount a partition.

            sudo mount /dev/xvdf1 /data 

To unmount a volume, use the below command.

         sudo unmount /dev/xvdf /data
         
         sudo unmount /dev/xvdf1 /data
