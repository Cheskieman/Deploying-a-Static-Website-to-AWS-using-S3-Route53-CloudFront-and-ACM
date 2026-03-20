# Deploying-a-Static-Website-to-AWS-using-S3-Route53-CloudFront-and-ACM

##  A complete step-by-step guide for launching a secure and high-performance static website on AWS using Amazon S3, CloudFront, and ACM

### This project will demonstrate how to:

*Set up an S3 bucket to deploy a static website

*Create a certificate for your domain from Certificate Manager 

*Create a CloudFront Distribution to host the S3 Static Website

*Configure a Route 53 DNS record to route the domain to a CloudFront distribution


#### Step-by-Step instruction guidance

**Set up an S3 bucket to deploy a static website**

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
*Select Create Bucket at the bottom.
<p align="center">  
  <img src="resources/Select Create Bucket initial.png" alt="Select Crete Bucket" width="900" />  
</p>  
*Select the recently created Bucket
<p align="center">  
  <img src="resources/click on recently created s3 bucket.png" alt="Select recently created Bucket" width="900" />  
</p>  
*Select the Upload button from the right
<p align="center">  
  <img src="resources/select upload for s3 bucket content.png" alt="Upload Files" width="900" />  
</p>  
*Select the Add files button
<p align="center">  
  <img src="resources/select add files to s3 bucket.png" alt="Add Files" width="900" />  
</p>  


*Select the files for uploading( one should include an index.html file)

*Select Upload from the bottom
<p align="center">  
  <img src="resources/select upload for s3 bucket content.png" alt="Select Upload" width="900" />  
</p>  
 
 **Create a certificate for your domain from Certificate Manager**

*Select by typing Certificate Manager from the AWS Searchbar
<p align="center">  
  <img src="resources/select certificate manager from aws searchbox.png" alt="Select Certificate Manager from AWS Searchbar" width="900" />  
</p>  
 *Make sure the region is the same as the S3 Bucket that was created
<p align="center">  
  <img src="resources/confirm certificate manager location is in same region as s3 bucket.png" alt="Same region" width="900" />  
</p>  
 *Select the Request button on the right
<p align="center">  
  <img src="resources/Select request for certificate.png" alt="Select Request button" width="900" />  
</p>  
 *Select Request a public certificate
<p align="center">  
  <img src="resources/Select request a public certificate.png" alt="Select Request Public Certficate" width="900" />  
</p>  
 *Select Next at the bottom of the page
<p align="center">  
  <img src="resources/Select next certificate setup.png" alt="Select Next" width="900" />  
</p>  
 *Select a name for a fully qualified domain name
<p align="center">  
  <img src="resources/add name for fully qualified domain name set up public cerficate.png" alt="Select Fully Qualified Domain Name" width="900" />  
</p>  
 *Select the Request button at the bottom
<p align="center">  
  <img src="resources/Select request button at the bottom.png" alt="DNS Resolution Command" width="900" />  
</p>  
 *Select the recently created certificate
<p align="center">  
  <img src="resources/Recently created certificate.png" alt="Select Request" width="900" />  
</p>  
 *Select the Create records in Route 53 button
<p align="center">  
  <img src="resources/click create records route 53 button.png" alt="Select Create Records in Route 53 " width="900" />  
</p>  
 *Select the Create records button
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p>  

**Create a CloudFront Distribution to host the S3 Static Website**

*Select by typing CloudFront from the AWS Searchbar
<p align="center">  
  <img src="resources/Select Cloudfront from Searchbar.png" alt="Select CloudFront from AWS Searchbar" width="900" />  
</p> 
*Select Create Distribution
<p align="center">  
  <img src="resources/Give Distribution a name.png" alt="Give Distribution a name" width="900" />  
</p> 
*Give the Distribution a name
<p align="center">  
  <img src="resources/Give Distribution a name.png" alt="Give Distribution a name" width="900" />  
</p> 
*Select  Next at the bottom
<p align="center">  
  <img src="resources/Click next .png" alt="Click Next" width="900" />  
</p> 
*Select Amazon S3 as the Origin Type
<p align="center">  
  <img src="resources/Select S3 origin.png" alt="Select S3 as records type" width="900" />  
</p> 
*Select the Browse S3 and select the S3 bucket created earlier 
 <p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select Next at the bottom
<p align="center">  
  <img src="resources/Click next .png" alt="Select the Next Button" width="900" />  
</p> 
*Select Enable security protections for the Web Application firewall
<p align="center">  
  <img src="resources/Click next .png" alt="Select the Next Button" width="900" />  
</p> 
*Select Next at the bottom
<p align="center">  
  <img src="resources/Click next .png" alt="Select Next " width="900" />  
</p> 
*Select the Create distribution button at the bottom
<p align="center">  
  <img src="resources/Select Create Distribution initial.png" alt="Select Create Distributions" width="900" />  
</p> 
*Select the General tab
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Edit button
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Type the CNAME of the domain
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the certificate created earlier
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Type index.html for the Default root object
 <p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Save changes button at the bottom
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Origins Tab
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Behaviors tab
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Create behaviors button
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the asterisk symbol for the path pattern
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the S3 Bucket created earlier for Origins and origins groups
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Create behavior button at the bottom
 * Select the Create records button
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the circle next to the Origin name
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Edit tab
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Copy policy button and then press cancel at the bottom
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Return to the S3 bucket created earlier and open the Permissions tab
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Scroll down and select the Edit button from the Bucket policy window
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Paste the policy copied from earlier
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Save changes button
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 


**Configure a Route 53 DNS record to route the domain to a CloudFront distribution**


*Select by typing Route 53 from the AWS Searchbar
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
* Select Hosted zones from the left-hand navigation panel
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
* Select the Hosted zone that was created
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
* Select Create record
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select Alias to Cloudfront Distribution
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select "Alias to Cloudfront Distribution."
*Select the CloudFront Distribution created earlier
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Create records button
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Distribution domain name in the CloudFront Distributions tab and type it into the URL
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
*Select the Alternate domain name in the CloudFront Distributions tab and type it into the URL
<p align="center">  
  <img src="resources/select create records button.png" alt="Select Create Records" width="900" />  
</p> 
   

 
















##### Contribution Policy

This project is not accepting external contributions, including pull requests or feature requests.

It serves as a personal archive of my learning journey in applying foundational concepts in software development and version control. Active development is not ongoing, and external changes will not be integrated.

Thank you for your understanding.
