# Threat Detection & Response Using Microsoft 365 Defender.  

This project demonstrates a simulated enterprise security setup using Microsoft 365 E5 Developer Tenant and Azure Free Tier resources. The primary goal is to illustrate threat detection and response capabilities, apply Identity and Access Management (IAM) policies, explore Microsoft Sentinel's capabilities, and focus on compliance and hardening—all within the constraints of free-tier services.

# Table of Contents
* Project Objectives.
* Free Tier Services Utilized.
* Project Toolkit. 
* Step-by-Step Guide.
* Simulated Attack Results. 
* Compliance & Hardening Insights. 
* Conclusion. 

# Project Objectives. 

* Simulate Threats: Detect and respond to simulated threats, specifically phishing attacks, using Microsoft 365 Defender.
* Focus on Compliance & Hardening: Explore compliance posture and data loss prevention (DLP) features available through the Compliance Manager.
* Apply IAM Policies: Implement foundational Identity and Access Management policies with Azure Active Directory (Free Tier).
* Explore SIEM-lite: Utilize Microsoft Sentinel (within its free ingestion limits) for basic log analytics and security information and event management (SIEM) capabilities.
* Leverage Free Resources: Accomplish all objectives exclusively using Microsoft's free developer and Azure free-tier programs.

# Free Tier Services Utilized. 

| Service                    | Access Method           | 
| :------------------------- | :---------------------- | 
| Microsoft 365 Defender     | M365 E5 Dev Program     | 
| Azure AD (Free)            | Azure Portal            | 
| Microsoft Sentinel         | Azure Portal            |
| Compliance Manager         | M365 Compliance Center  | 
| Azure Resource Manager     | Azure Free Account      | 

## Project Toolkit

| Tool                      | Usage                                             |
| :------------------------ | :------------------------------------------------ |
| Microsoft 365 Defender    | Core focus: simulate & analyze attacks            |
| Microsoft Sentinel        | Connect logs for the SIEM-lite experience         |
| Azure AD Free Tier        | IAM policies & Conditional Access                 |
| Compliance Manager        | Review compliance posture & DLP testing           |
| GitHub + VS Code          | Documentation, repository, markdown authoring     |


###  Set Up Microsoft 365 Developer E5 Tenant
1. Go to: [Microsoft 365 Developer Program]. 
2.  Sign up and choose **“Instant Sandbox”** 
3.  This will grant access to:
    * Microsoft 365 Defender
    * 25 dummy users
    * Azure AD Free Tier
    * Compliance Center

  ###  Set Up an Azure Free Account

1.  Go to: [Azure Free Account]. 
2.  Sign up using the  email. 
3.  Access to Always-free services (e.g., Log Analytics workspace, Azure AD Free, Azure Functions).

###  Simulate a Phishing Attack via Defender

1.  Navigate to: [Microsoft 365 Security Portal]. 
2.  Go to **Attack Simulation Training**.
3.  Create a **Phishing Campaign** targeting 3–5 of your dummy users.
4.  Monitor and track the results:
    * User click rates on the phishing links.
    * Microsoft Defender's detection capabilities. 
    * Any auto-remediation actions taken by Defender.
  
###  Enable Microsoft Sentinel (Free Ingestion)

1.  In the Azure Portal, create a new **Log Analytics Workspace**.
2.  Enable **Microsoft Sentinel** on the newly created workspace.
3.  Connect the following data connectors:
    * **Microsoft 365 Defender** logs
    * **Azure Activity Logs**
4.  Create a simple analytics rule to demonstrate basic SIEM functionality:
    * Rule name: "Phishing Click Event"
    * Trigger: Based on logs indicating a phishing click detected by Defender.
    * Action: Configure an email alert to notify relevant personnel.
  

 ## Compliance & Hardening Insights.
 
  * Compliance Score Analysis. 
  * Initial score. 

## Key areas for improvement identified:

  * DLP Policy Testing. 

## Scenario for data exfiltration simulation:

  * Alerts generated by DLP. 

## Information Protection Labels. 

  * How labels could be used to protect data involved in the simulation.


## Screenshots 

![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/7cf9e895408e3bea45d481b93ad5eabcd21b4c75/Screenshot%202.png)

* Instant Sandbox” (recommended). 


![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/28f455f6c8054ab8000044a46889eb191869bed9/Screenshot%205.png)

* Add new groups on Azure portal. 

![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/9f9b128c8b91c08ac31ef67430ee0496152ab721/Screenshoots/Screenshot%201.png)

* Create log analytics workspace. 


![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/b368d9fd8de123673857d9c59cd1f30072433ac2/Screenshoots/Screenshot%202.png)

* Add microsoft sentinel to a workspace. 

![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/708a852a37cf0e121810ea15e3e4105de6e78786/Screenshoots/Screenshot%203.png)

* Subscription based microsoft defender for cloud. 

![iamge alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/f49a4316eab81767a13cceef5cdb7dea60bb1633/Screenshoots/Screenshot4.png)

* Analytics rule details. 


![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/4a794ad5e89f369d5e66d5b6ffe6fd1c241bd32a/Screenshoots/Screenshot%205.png)

* Select azure activity or azure active directory. On Microsoft sentinel for data connectors.

![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/4add563c56837d6638b687fe8077bb2fc77d2bbc/Screenshoots/Screenshot%207.png)

* Select Microsoft defender for office 356. On Microsoft sentinel for data connectors. Open conntors page. 



![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/53ecbaf659a886aae76d449001b165b53594f61d/Screenshoots/Screenshot%209.png)

* Results for "DLP Policies"

![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/817f572c23c55924bdf7f5d932cbbdd0289f1db4/Screenshoots/Screenshot%2010.png)



![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/7e098dab32cd8b05ec7f6b99cdf25ef05d29b261/Screenshoots/Screenshot%2011.png)

* Results for "Information Protection labels"


![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/96afb21bc2eaac1f699a1db332f744fbcbfe605c/Screenshoots/Screenshot12.png)

* Azure portal welcome page. 

![image alt](https://github.com/Md-Shabbir-ahamed/Threat-Detection-Response-Using-Microsoft-365-Defender/blob/475f9d1a1575f50e0c61f82b993fc8b4ca46fb2f/Screenshoots/Pic%2013.png)

* Azure activity data connetors conntected.


## Conclusion

This project successfully demonstrates the core capabilities of Microsoft 365 Defender, Azure AD, and Microsoft Sentinel within their respective free tiers. It provides a foundational understanding of how these tools integrate for threat detection, response, identity management, and compliance in a simulated enterprise environment.

## License

This project is open-source and available under the MIT License.


