<h1 style="text-align: center;">Introduction to Amazon Elastic Block Store (EBS)</h1>

----

**Amazon Elastic Block Store (EBS)** is a block storage service provided by Amazon Web Services (AWS). It is designed to provide persistent block-level storage volumes for use with Amazon EC2 instances. EBS volumes are highly available and reliable, offering durable storage for applications and data in the cloud.

### Benefits
- **High Performance**: EBS volumes offer consistent and low-latency performance, making them suitable for a wide range of workloads, including databases, enterprise applications, and data analytics.
- **Scalability**: Users can easily increase or decrease the size of EBS volumes on the fly without impacting running applications, providing scalability to meet changing storage requirements.
- **Snapshot Backup**: EBS supports point-in-time snapshots, allowing users to create backups of volumes for data protection and disaster recovery purposes.

- **Flexibility**: EBS offers different volume types.


### There are different volume types in EBS :
- **General Purpose (SSD)**: Suitable for a wide variety of workloads, providing balanced performance and cost.
- **Provisioned IOPS (SSD)**: Designed for I/O-intensive workloads that require consistently high performance.
- **Throughput Optimized (HDD)**: Optimized for frequently accessed, large datasets with high throughput requirements.
- **Cold HDD**: Ideal for infrequently accessed workloads, offering low-cost storage for large volumes of data.
___
<br>
<h3>1. Creating an EBS Volume </h3>
<br>

Step1 : Sign in to the AWS Management Console.
![](./image%20src/step1.png)
<br>


Step2 : Navigate to the EC2 dashboard.
![](./image%20src/step2.png)
<br>


Step3 : Click on "Volumes" in the left sidebar.
![](./image%20src/step3.png)
<br>


Step4 : Click on "Create Volume."
![](./image%20src/step4.png)
<br>

Step5 : Select the desired volume type, size, availability zone, and other configuration options.
![](./image%20src/step5.png)
<br>


Step6 : Click on "Create Volume."
![](./image%20src/step6.png)

<br><h3>2. Attaching and Detaching EBS Volumes </h1>

Step1 : Navigate to the "Instances" section of the EC2 dashboard and create the instance
![](./image%20src/Attach_step1.png)
<br>

Step2 : Navigate to the volumes and choose the volume which you want to attach and detach.
![](./image%20src/Attach_step2.png)
<br>

Step3 : Click on "Actions" and then "Attach Volume."
![](./image%20src/attach_step3.png)
<br>

Step4 : After clicking on attach volume select the instance, device name and then attch the volume
![](./image%20src/attach_step4.png)
<br>

<h3>3. Using EBS Snapshots</h3><br>
EBS snapshots are point-in-time backups of EBS volumes. They are crucial for data backup and recovery. <br>
<h3>To create a snapshot</h4><br>
 
Step1: Navigate to the EBS volume in the AWS Management and  Click on create snapshot.
![](./image%20src/snapshot1.png)
<br>

Step2: Select the volume.
![](./image%20src/snapshot2.png)
<br>

Step3: Click on create snapshot.
![](./image%20src/snapshot3.png)
<br>

<h3>4. EBS Encryption</h3>

Encrypting an EBS (Elastic Block Store) volume is essential for ensuring the security of data stored in the AWS cloud. Encryption helps protect data at rest and in transit, safeguarding it from unauthorized access or breaches.<br>

<h5>To enable encryption for an EBS volume</h5><br>

Step1: Select the unencrypted volume.
![](./image%20src/encrypt1.png)
<br>
Step2: Create the snapshot of the selected volume.
![](./image%20src/encrypt2.png)<br>

**Note :** An unencrypted volume will create an unencrypted snapshot and vice versa.

![](./image%20src/encrypt3.png)<br><br>
Step3: Create the volume from the newly created snapshot.

![](./image%20src/encrypt4.png)<br>
![](./image%20src/encrypt5.png)<br>
![](./image%20src/encrypt6.png)<br>
![](./image%20src/encrypt7.png)<br><br>


Step 4: Navigate to the volume option where you can find the newly created encrypted volume.
![](./image%20src/encrypt8.png)<br><br>

<h3>5. Cleaning Up</h3>

To avoid unnecessary costs, it's important to delete EBS volumes and snapshots when they're no longer needed.
Regularly review your EBS resources and delete any unused ones.

##### Steps to delete the snapshots

Step1: Navigate to snapshots. Select the snapshot and clickon delete snapshot.
![](./image%20src/SnapShotdel1.png)<br>

Step2: Click on delete button.
![](./image%20src/SnapShotdel2.png)<br><br>

##### Steps to delete the volume

Step 1: Navigate to volume. Select the volume, click on action and then detach the volume.
![](./image%20src/voldel1.png)<br>

Step 2: Click on **detach** button.
![](./image%20src/voldel2.png)<br>

Step 3: Select the volume, click on action and then delete volume.
![](./image%20src/voldel3.png)<br>

Step 4: Click on the **delete** option, and the volume will be deleted successfully.
![](./image%20src/voldel4.png)<br>

----
Congratulations!!, You have successfully completed the lab!