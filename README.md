# MySQL docker

### **Description**

This will create a dockerized for MySQL:

-  **mysql**, MySQL database container ([mysql](https://hub.docker.com/_/mysql/) official Docker image)

### **Install Docker Desktop on Windows**
-  https://docs.docker.com/desktop/windows/install/

-  Check
```
Windows + R -> cmd -> ENTER
```
```
C:\Users\Administrator>docker -v
Docker version 20.10.6, build 370c289
OK!

C:\Users\Administrator>docker-compose -v
docker-compose version 1.29.1, build c34c88b2
OK!
```
#### **Download & install GIT**
https://git-scm.com/download/win
-> 64-bit Git for Windows Setup

Create new folder
Right Click
Run Git Bash Here
Run commands
```
git clone https://github.com/hatt732/mysql-docker-win10.git
cd mysql-docker-win10
```

#### **Run MySQL**
```
docker-compose up -d
```
#### **Connecting with MySQL Workbench**

```
    DB_HOST=mysql
    DB_PORT=13306
    DB_DATABASE=appdb
    DB_USERNAME=user
    DB_PASSWORD=userpassword
    MYSQL_ROOT_PASSWORD=root
```

#### **Directory Structure**
```
+-- mysql5.7 <project root>
|   +-- docker-compose.yml
+-- readme.md <this file>
```

**Default configuration values** 

The following values should be replaced in your `.env` file if you're willing to keep them as defaults:
    
    DB_HOST=mysql
    DB_PORT=13306
    DB_DATABASE=appdb
    DB_USERNAME=user
    DB_PASSWORD=userpassword
    MYSQL_ROOT_PASSWORD=root
    
