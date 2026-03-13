# Deploying-a-Static-Website-to-AWS-using-S3-Route53-CloudFront-and-ACM

##  A complete step-by-step guide for launching a secure and high-performance static website on AWS using Amazon S3, CloudFront, and ACM

### This project will demonstrate how to:

*Set up an S3 bucket and (possibly: deploy a static website)


#### Step-by-step Instruction guidance

**Set up an S3 bucket and (possibly: deploy a static website)**

*Select by typing S3 from the AWS Searchbar 
<p align="center">  
  <img src="resources/select s3 from aws searchbox.png" alt="Type S3 from AWS Searchbar" width="900" />  
</p>  
*Select Create Bucket
<p align="center">  
  <img src="resources/Select Create Bucket initial.png" alt="Select Create Bucket" width="900" />  
</p>  
*Give the S3 bucket a name
<p align="center">  
  <img src="resources/Give bucket a name.png" alt="Give S3 Bucket a name " width="900" />  
</p>  
*Deselect the Block all public access box and select the acknowledged box 
<p align="center">  
  <img src="resources/Unblock and acknowledge s3 bucket.png" alt="Deselect Block Public Access & Acknowledgement S3" width="900" />  
</p>  
*Select Create Bucket at the bottom.
<p align="center">  
  <img src="resources/Select Create Bucket initial.png" alt="Select Crete Bucket" width="900" />  
</p>  
* Select the recently created Bucket
<p align="center">  
  <img src="resources/click on recently created s3 bucket.png" alt="Select recently created Bucket" width="900" />  
</p>  
* Select the Upload button from the right
<p align="center">  
  <img src="resources/select upload for s3 bucket content.png" alt="Upload Files" width="900" />  
</p>  
* Select the Add files button
<p align="center">  
  <img src="resources/select upload for s3 bucket content.png" alt="Add Files" width="900" />  
</p>  
* Select the files for uploading( one should include an index.html file)

* Select Upload from the bottom
<p align="center">  
  <img src="resources/select upload for s3 bucket content.png" alt="Select Upload" width="900" />  
</p>  
 
 **Request a Certificate from Certificate Manager**

 * Select by typing Certificate Manager from the AWS Searchbar
<p align="center">  
  <img src="resources/select certificate manager from aws searchbox.png" alt="Select Certificate Manager from AWS Searchbar" width="900" />  
</p>  
 * Make sure the region is the same as the S3 Bucket that was created
<p align="center">  
  <img src="resources/confirm certificate manager location is in same region as s3 bucket.png" alt="Same region" width="900" />  
</p>  
 * Select the Request button on the right
<p align="center">  
  <img src="resources/Select request for certificate.png" alt="Select Request button" width="900" />  
</p>  
 * Select Request a public certificate
<p align="center">  
  <img src="resources/Select request a public certificate.png" alt="Select Request Public Certficate" width="900" />  
</p>  
 * Select Next at the bottom of the page
<p align="center">  
  <img src="resources/Select next certificate setup.png" alt="Select Next" width="900" />  
</p>  
 * Select a name for a fully qualified domain name
<p align="center">  
  <img src="resources/add name for fully qualified domain name set up public cerficate.png" alt="Select Fully Qualified Domain Name" width="900" />  
</p>  
 * Select the Request button at the bottom
<p align="center">  
  <img src="resources/Select request button at the bottom.png" alt="DNS Resolution Command" width="900" />  
</p>  
 * Select the recently created certificate
<p align="center">  
  <img src="resources/dns server resolution command and output.png" alt="Select Request" width="900" />  
</p>  
 * Select the Create records in Route 53 button
<p align="center">  
  <img src="resources/click create records route 53 button.png" alt="Select Create Records in Route 53 " width="900" />  
</p>  
 * Select the Create records button
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p>  
   

 
















##### Contribution Policy

This project is not accepting external contributions, including pull requests or feature requests.

It serves as a personal archive of my learning journey in applying foundational concepts in software development and version control. Active development is not ongoing, and external changes will not be integrated.

Thank you for your understanding.
