# Beyond_Repo_Project
The web application is Gohst CMS buit on NODEjs. The applaci=tion usues docaker for the site the site files and a seoerate container for the maria DB database. The containers data of the site is kept is persistent as theu =y are mounted to the host volumes. The  files that agenerated are sunced  then backed up to AWS s3 via crontab at 5 minuet intervals 

the two options I had to  was 1 to hard back the AWS 



This template deplos the App into the environment.

I thoought about using a a RDS data base however I thought to challenge myselfa .

The outcome was to use maria DB in containers that  are backed up to the host machine and then to the s3
