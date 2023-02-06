# demo-config-server


Azure Monitoring Agent OvERVIEW :
=====================


  WINDOWS  																														Linux 
 - WAD(WINDOW DIAGNOSTIC) 	-
	  Az resruces ,Storege Account , Az monitoring agenet ,Event Hubs 
																														-LAD(Linux Dig)
 -LAW(Log Analytics workspace agent)-
 Azzure Resources ,3rd party cloud ,AWS ,ONPreme, Az Monitor Logs														LAW agent 
  Sentinel ASC
 -Dependecy agent 																										Depe Agent 
		Azzure Resources ,3rd party cloud ,AWS ,ONPreme																	Telegraph AgENT 
		Dependecy aganet like network 
		 Az monitoring logs 
3 types:
		Log Analytics Agent (Azzure Resources ,3rd party cloud ,AWS ,ONPreme)
		Dependecy Agent 
		Telegraph Agent 

Home>Monitor
1:Create Data Collection Rule:
============================

to pump data into Azure monitor 


New service : Azure monitor controll service (Heart of monitor)


Collect text logs with Azure Monitor Agent;

metrics:
https://<azure_region_code>.monitoring.azure.com


System asssigned managed identity :
==================================
   
Home>Monitor>Data Colection Rules > CustomLogCapture >DataSources>


Sending Logs From A Linux Server to Log Analytics Workspace in Azure:
===================================================================

Home>Log Analalytics workspace >Create>


Create log analytics workspace :
parameters 
  Resource group :304-test
  Instance name: SendLinuxVMLogs
  
   click on create and submit , will take few minutes 
check :
Home>Log Analalytics workspace>
select -SendLinuxVMLogs>

>Agent management 

Heartbeat | where OSType == "Linux"

Heartbeat | count
