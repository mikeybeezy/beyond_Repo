#Summary
The web application is Ghost CMS. Ghost is an open source publishing platform built on NODEjs. The application uses Docker container and a separate Docker container to run a Maria DB Mysql database. The data generated via  containers are kept persistent and mounted to host volumes. The files that are generated by users are synced then backed up to AWS S3 via crontab at 5 minuet intervals. The application can be deployed by itself into any AWS environment through cloud formation script. The application environment can also be deployed with the application.


#Overview of what was achieved
Setup an ubuntu 16.04 box. Used docker containers to host a Node.js application. Used Docker To host a Maria DB container. Synced and replicated the content to AWS S3 Replicated content from AWS S3 to the Ubuntu Box that hosts the Docker containers Created an AWS environment to deploy the application into

#Challenges
Deciding whether to use RDS or Docker container for the application Database. I opted to go with the Docker container option as I felt it it would allow me to learn more about how the technology worked and eventually progress to kubernetes. Some of the challenges I faced include finding the most efficient method to maintain and manage persistent data across all platforms and instances. orchrastrating the implementation of automation with as little human intervention as possible. Having to decide whether to pre bake Ubuntu AMI's with all necessary settings and configs or automating  all installation and configuration on demand.
