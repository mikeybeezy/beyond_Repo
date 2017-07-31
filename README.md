# Beyond_Repo_Project
The web application is Gohst CMS. Ghost is an open source publishing platform buit on NODEjs. The applaci=tion usues docaker for the site the site files and a seoerate container for the maria DB database. The containers data of the site is kept is persistent as theu =y are mounted to the host volumes. The  files that agenerated are sunced  then backed up to AWS s3 via crontab at 5 minuet intervals 

the two options I had to  was 1 to hard back the AWS 

This template deplos the App into the environment.

I thoought about using a a RDS data base however I thought to challenge myselfa .

The outcome was to use maria DB in containers that  are backed up to the host machine and then to the s3

# Overview of what was achieved
Setup an ubuntu 16.04 box
Used docker containers to host a Node.js  application
Used Docker To host a Maria DB container 
Synced and replicated the content to S3
Replicated Content from AWS S3 to The Ubuntu BoX that hosts the Docker containers
Created an AWS environment to deploy the application into

# Challenges
Some of the challenges I face include
Finding the most efficient to maintain and manage persistent data across all platforms and instances
orchrasting the implementiiopn of automation with as little human interacion as possible

