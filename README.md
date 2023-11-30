# vprofilesetup-local-

## Setting up a Multi Tier Web Application locally

### Project Architecture
![Screenshot 2023-11-29 at 3 48 33 PM](https://github.com/zubujams/vprofilesetup-local-/assets/52971863/a3a7b1f0-c79b-4cc1-908f-e302da906471)

### 1. Users access application -- when users login the application runs an SQL query on a MYSQL database to get login information

### 2. Connect to the NGINX loadbalancer

### 3. Requests are then routed to an Apache Tomcat server (a JAVA webapp service). With an external NFS server.

### 4. Rabbit MQ is connected to Tomcat - a message broker used to connect apps together.

### 5. Before the users requests goes to the MYSQL database it will go through memcache database caching service

### Automation stack - Vagrant + Oracle VM virtual box + Bash scripts and commands = Sets up the above services

![Screenshot 2023-11-29 at 7 11 12 PM](https://github.com/zubujams/vprofilesetup-local-/assets/52971863/e171d24f-b8b1-4c13-a5b7-7274896d133f)

