Creating a Custom AI Agent for Analyzing Azure Tagged Questions on Microsoft Q&A Forum
Harnessing AI to Gain Insights from Community Interactions
Link to the Agent: Overview - PinnacleHomeworkCopilot | Microsoft Copilot Studio
(Please let me know if you could not access it and how we can grant the same adhering security guidelines)

Building the Copilot Studio Agent 
•	In Copilot Studio, create Agent with name as “PinnacleHomeworkCopilot” as shown below:
 
•	Add Description as: Get analytics of Azure tagged questions asked over Microsoft Q&A forum
•	Add Instructions as: 
- Get all supported Azure tags from Microsoft Q&A forum 
- Analyse the questions asked for Azure Databases Service Area 
-Check the most used Azure services tags from the questions 
-Provide accurate and direct responses while minimizing unnecessary details.

•	Adding your knowledge base to the Agent:

Use Microsoft Q&A forum site to serve as Knowledge base to Agent:
Microsoft Q&A | Microsoft Learn
Since the website cannot be more than two levels deep, we will consider upto 2nd level:
 


•	Once Knowledge base is added, we will test agent by asking questions like below:
 

We will refine questions more like specific Azure tags like “Azure SQL Database”, or Month-wise.
Since model is having data only till October 2023, it did not return back the output:

 
•	Send Email to Outlook by adding Action:

 

We will connect to Office365 if not already connected in “Manage your connections”

 
 

Update the Agent’s Instructions and Send the email:
 

Make sure Orchestration is Enabled.

Give prompt as below “share it with **emailed**”

 

Question asked on Azure Data Factory for which Output is sent to email id shaktisingh@microsoft.com

Result in Outlook Inbox:

 
