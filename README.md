# Assignment_3 --> Assignment on Testing, Linux and Servers

**Task #1** - System Monitoring Setup

Step 1: Creating a Monitoring directory

  ![image](https://github.com/user-attachments/assets/874322f3-3868-4e05-8145-31f72cd9cd6a)
    
Step2:  Install htop sudo apt update
  ![image](https://github.com/user-attachments/assets/90e34e54-eee0-44ff-b594-4a90b5ba43fa)

Step2A: Running the Htop Command - shows the various logs  
  ![image](https://github.com/user-attachments/assets/2770d9e3-254e-4f8d-9afa-c0b8c23197de)

Step3: Installing nmon
![image](https://github.com/user-attachments/assets/9f562319-de73-49ed-86fa-5a77378e3790)

Step3A: checking for CPU

![image](https://github.com/user-attachments/assets/43e32c7c-383e-48b5-be46-ee0c8cdeae9a)

Step3B: checking for memory

![image](https://github.com/user-attachments/assets/16b0535a-e95b-49d1-8c31-5acb5b641847)

Step4: disk usage monitoring to track storage availability using df and du.

Step4A: **Disk Usage**

![image](https://github.com/user-attachments/assets/508f7a0c-5039-4b37-9bc1-7f523f95e8de)

Step4B: **Disk File System**

![image](https://github.com/user-attachments/assets/d6cb64f9-dd23-432c-9c3f-086754a9bc1b)

Step5: Identify resource-intensive applications. top 15 cpu utilizations

![image](https://github.com/user-attachments/assets/ebc8076f-da2a-4cf0-b297-27e45a6dff58)

Step6: Cron Job (shell scripting) for every 5 mins. 

![image](https://github.com/user-attachments/assets/d8495cab-33fb-4b4f-92b0-fe621e0acb51)

Step6A: Contents of Reporting Log File 
![image](https://github.com/user-attachments/assets/22af129b-4a33-4b55-94c1-1f633c24b007)

Step6B: After a sucessfull cron job execution(Every 5 mins)
![image](https://github.com/user-attachments/assets/b60f9c06-cf31-48d8-9a95-e7cc892ab870)

Step6C:Opening the file

![image](https://github.com/user-attachments/assets/5c8f7da3-a640-4d4f-afee-62c9c6eebea3)

End of Task #1 

*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*

Start of Task #2

Step1: User (Sarah & Mike) Creation

![image](https://github.com/user-attachments/assets/1786371a-21d3-4d2e-af69-fb618e784594)

Step2: Creating a password for the newly created Users 

![image](https://github.com/user-attachments/assets/b026e1fe-f20b-48ac-8548-c2e2de15bcea)

Step3: Creating Dedicated Workspace Directories

![image](https://github.com/user-attachments/assets/3496197e-b9f8-4316-8958-81545f152a95)

Step4: Seting up the Proper Ownership & Permissions, for Owner Access Only.

![image](https://github.com/user-attachments/assets/70203d69-ad40-4b43-ba2f-f03fff0d7240)


Step 5: Password Expiry Policy (should expire in 30 Days)

![image](https://github.com/user-attachments/assets/38061d64-866e-4a05-9eb5-7c8c11fea2d6)

End of Task #2

*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*

Start of Task #3

Step1: Create Backup Destination Directory

![image](https://github.com/user-attachments/assets/e30ccc00-1ff4-48cd-9995-860f420c6855)

Step2: Creating Backup Scripts

For Sarah, since she is using Apache Servcers, the backup file created is apache_backup.sh
![image](https://github.com/user-attachments/assets/24491eb1-dc01-4f9f-b802-76df8aca8f88)

For Mike, since he is using nginx servers, the backup file created is nginx_backup.sh
![image](https://github.com/user-attachments/assets/4208eec1-3424-4143-9577-c5e2b7b44026)

Setting executable permissions

![image](https://github.com/user-attachments/assets/671164f6-cc31-41c4-8cdc-b1fc6ba676fe)

Switching to Sarah user and enabling the Cronjon at the crontab 
![image](https://github.com/user-attachments/assets/d652a13d-e768-42b3-bdb0-76187bd207ac)
![image](https://github.com/user-attachments/assets/43905a9c-c03f-4c85-8cc5-58063be0bc33)

Switching to Mike user and enabling the Cronjon at the crontab
![image](https://github.com/user-attachments/assets/89898dc4-0de3-48da-bb66-2c60e58429dc)
![image](https://github.com/user-attachments/assets/4fd917cb-ef28-4023-98c7-0a30bb1d50c4)

Running the backfile for (Sarah)apache and verifying the log file.
![image](https://github.com/user-attachments/assets/22bfc831-9bd8-427a-97ce-4d8219cafa26)

Running the backfile for (Mike)nginx and verifying the log file. 
![image](https://github.com/user-attachments/assets/74fa8974-84c1-4ad4-885e-6debd34179f4)










