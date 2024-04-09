# Microsoft Defender

![image](https://github.com/Ashrafs-Tech/Microsoft-Defender/assets/166546026/7358da11-4196-4d25-829d-9903bf300768)

## Intro

I will enable Microsoft Defender for Cloud because it will give me a high level of my Azure environment in terms of security.

And it will let me take logs from my Linux and Windows virtual machines along with the logs from each of their Network Security Groups so they can be forwarded into the Log Analytics Workspace.

But that's for the next step.

## Setting up Defender for Cloud for virtual machines, SQL, and data collection:

- Make sure both Linux and Windows virutal machines are running.
- In the Azure bar, search for Microsoft Defende for Cloud
- Click Environment Settings
- Find Law-Cyber-LAV-Ver1 and click "..."

  ![image](https://github.com/Ashrafs-Tech/Microsoft-Defender/assets/166546026/f5038eb5-0554-4e88-b740-599a6390ad09)

- After that, turn on servers and SQL servers on machines
- Enable Defender Plans
- Click Save
  * This will allow me to collect logs from the virtual machines and SQL Server

  ![image](https://github.com/Ashrafs-Tech/Microsoft-Defender/assets/166546026/1071ece3-0c11-4d25-963c-5d1655d84665)

- After that, I went to Data Collection.
- I clicked All Events and then clicked Save
  * This will let me collect from Windows Security log
  * It will let me see people attempting to login into my Windows machine

 ![image](https://github.com/Ashrafs-Tech/Microsoft-Defender/assets/166546026/9a61d4ed-de68-4f44-b7de-38a4582e1b47)

 ## Set up Defenhder for Cloud for Subscriptions

- In the Azure bar, search for Microsoft Defende for Cloud
- Click Environment Settings
- Find Azure Subscription 1 and click "..."

![image](https://github.com/Ashrafs-Tech/Microsoft-Defender/assets/166546026/bdf6e033-8d96-4c27-b647-b81b2a48211b)

- In Defender plans, turn on the following:
  * Servers
  * Database
  * Storage accounts
  * Key Vault
  * Click Save
 
![image](https://github.com/Ashrafs-Tech/Microsoft-Defender/assets/166546026/d1b0f10c-b871-4d0e-9ff7-881e4da13e34)


## Enable MS Defender for Cloud Continuous Export

While on the same page:

- Clicked on "Continuous export"
- Then clicked on "Log Analytics Workspace"
- Turn on Exports Enabled
  * This will export alerts into the Log Analytics Workspace and be able to query them for later
     - For example, if Defender for Cloud finds a problem in my environment like a brute force attack or theres a poor configuration, these export those alerts in the central repository.
- Check all the boxes
  * Security Recommendations
  * Secure Score
  * Security alerts
  * Regulatory compliance
    - This in particular will enable NIST SP 800-53 for the environment to see which controls are missing.
- I made sure it was set to the correct Resource Group "RG-Cyber-Lab"
- The target workspace is "Law-Cyber-Lab-Ver1"
- And clicked Save

![image](https://github.com/Ashrafs-Tech/Microsoft-Defender/assets/166546026/7b2ee077-54e3-4c92-9363-0eb4799c3e69)
![image](https://github.com/Ashrafs-Tech/Microsoft-Defender/assets/166546026/bd323143-d533-448d-967b-b31ed10f6234)

## Step 4 is done.  
- Defender for Cloud was set up for:
  * Subscriptions
  * Virtual Machines
  * SQL Servers
  * Data Collection
- Alerts and Logs will be sent to the Log Analytics Workspace

![image](https://github.com/Ashrafs-Tech/Microsoft-Defender/assets/166546026/ce9adfc9-4cab-4eae-807c-842808793f8a)


 


