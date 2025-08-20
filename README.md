# Mini-Project-1-30-Day-MyDFIR-Microsoft-Challenge

#Outline 
1.	Current lab environment
2.	list out the resources 
3.	Progress Documentation 
4.	Reflection on Your Setup & KQL
5.	Reflection Points

# 1.	current lab environment 

<img width="1024" height="1536" alt="current lab" src="https://github.com/user-attachments/assets/14c35034-dced-4b65-b564-e2dd75199c14" />

# 2.	list out the resources 

1.	Azure Subscription 	        --> azure Subscription 1
2.	Resource Group 		          --> MYDFIR-shahid-RG
3.	Virtual Machines 		        -->  MYDFIR-shahid-VM
4.	log analytics workspace     --> Mydfir-shahid-law
5.	Sentinel workspace         -->  Mydfir-shahid-law
6.	data connectors 
      a. Azure Activity
      b. Microsoft sentinel training lab solution
      c. install Microsoft defender for XDR
7.	workbooks
      a.  Investigation insights



# 3. Progress Documentation 

Data Connectors Configured
•	Azure Activity: Connects the subscription-level audit log for all write operations.

•	Microsoft Defender for XDR (formerly Microsoft 365 Defender): This is a critical connector. It ingests alerts and raw data from Microsoft 365 (e.g., Microsoft Defender for Office 365, Microsoft Defender for Endpoint).

•	Microsoft Sentinel Training Lab Solution: This is a package that deploys sample data, analytic rules, hunting queries, and a workbook to simulate attack scenarios for learning purposes. Excellent for practice!


**Sentinel Components **

**Analytics Rules Created (These likely came with the Training Lab)**

<img width="749" height="347" alt="analytics rules created" src="https://github.com/user-attachments/assets/cb24d76c-d3a7-4489-a979-334000051ef9" />

**• Incidents Generated (These will be generated from the Training Lab rules)**

<img width="773" height="307" alt="incident generated" src="https://github.com/user-attachments/assets/0bb07d29-29c5-4f4d-b672-4abdb82d2ce3" />

**• Incident investigation **
<img width="772" height="379" alt="incident investigation" src="https://github.com/user-attachments/assets/100d0f4d-6215-4843-8c91-fde688730335" />

• Workbooks Created 
<img width="929" height="338" alt="created workbooks" src="https://github.com/user-attachments/assets/d32c1a93-9821-4418-a4b8-755612d362fd" />

**Dashboards **

**Bar chart**

<img width="626" height="308" alt="bar chart " src="https://github.com/user-attachments/assets/2b13a473-c3b9-47dd-810e-e4830a199735" />


**Pie Chart**

<img width="733" height="239" alt="pie chart " src="https://github.com/user-attachments/assets/43b3e1ba-c324-4d01-bd91-323e0486a252" />

# 4. Reflection on Your Setup & KQL
Since your setup includes the Training Lab, you have a perfect playground. Here’s an example of a KQL query you might run to investigate a simulated attack from the lab data.

. **advance hunting **

<img width="671" height="280" alt="advance hunting" src="https://github.com/user-attachments/assets/2e0cdb21-53ba-47c3-845b-ca3bed474b2d" />

. **Kql Query **

<img width="443" height="295" alt="kql query" src="https://github.com/user-attachments/assets/f463cd25-1668-4b03-9b30-2c750485c4af" />

# 5. Reflection Points

1. What was the most challenging part of the setup?
The most challenging part is often understanding the hierarchy and dependencies: ensuring the Virtual Machine and Log Analytics Workspace are in the same Resource Group and Region, and correctly enabling Sentinel on the workspace, not the resource group. Connecting the data connectors and ensuring they are ingesting data properly can also have a learning curve.

2. What was the most valuable thing you learned so far?
The most valuable insight is understanding the core architecture of a cloud SIEM: how data sources (like Azure Activity, M365) are connected via connectors to the Log Analytics Workspace, and how Sentinel sits on top to provide security analytics. It makes the theory of data ingestion and normalization very practical.

3. What are you most excited to work on in the next module?
I am most excited to dive into the Microsoft Sentinel Training Lab data. Using the pre-built analytic rules to generate incidents and then investigating them through the incident graph and hunting experience is the best way to learn real-world cyber investigation skills in a safe, simulated environment. 

