# Connecting with AWS

## Installation on AWS

- Node.js
- npm
- Mongo DB

## Installation on PC (for windows)

- putty.exe (ssh client)
- puttygen.exe (convert Amazon's .perm key pair file to .ppk file)
- WinSCP (GUI of transferring files between PC and AWS)

## EC2 Information

- Instance : i-04532a4e10ff1c9eb
- Public DNS : ec2-35-161-177-232.us-west-2.compute.amazonaws.com
- Public IP : 35.161.177.232
- Private DNS : ip-172-31-29-61.us-west-2.compute.internal
- Private IPs : 172.31.29.61

## Connect with AWS (for Mac)

- Please check http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html

## Change all default IP addresses in our app into EC2 public DNS to accomplish using server in AWS.

## How to

  Follow the steps in the first link (remember to install node.js with version after 4.0.0, otherwise npm cannot be successfully installed).

  When you finally access into AWS remote terminal, first check versions of node.js and npm using :

  '''
  node -v
  npm -v
  '''

  Then start Mongo DB using :

  '''
  sudo service mongod start
  '''

  Remember to create database :
  '''
    mongo
  > use node-login
  > db
  > db.getCollection('users').createIndex({"email":1}, {unique:true})
  '''

  Don't forget to use WinSCP to transfer necessary files to AWS.

  Go into "android-login-registration-authentication-server/node-login" and "ProjectRTC-master" and run servers :
  * node app.js

  Finally, you can run our app!

## Reference Links for Set Up and Downloads
- http://iconof.com/blog/how-to-install-setup-node-js-on-amazon-aws-ec2-complete-guide/
- http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html
- https://docs.mongodb.com/v3.0/tutorial/install-mongodb-on-amazon/