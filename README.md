![img](https://i.imgur.com/8lw3y7S.png)

# Objective 
The objective of this lab will focus on how to use the NIST 800-61 Incident Management Lifecycle to respond to alerts and potential threats within our Microsoft Sentinel. 

# NIST 800-61 Incident Management Lifecycle

![img](https://i.imgur.com/lwKdT0k.png)

# Step 1: Preparation
During the "Preparation" phase, an organization will take proper security precautions and measurements to make sure their system is equipped with incident response capabilities. An example of this would be, setting up and deploying a SEIM that will capture incidents and aggregate logs from various resources within the organization network. Other examples of this might include, creating an incident response plan and playbook, defining crucial roles and responsibilities within an incident response team, and/ or developing effective user training within your organization. 

# Step 2: Detection and Analysis
During "Detection and Analysis", analysts will actively look for potential threats and analyze the data they uncover. In this section, we'll walk through what the "Detection and Analysis" phase looks like within our Microsoft Sentinel

<H3> Detection and Analysis in Microsoft Sentinel </H3>

In this example, we're going to be investigating for any brute-force attacks being attempted on the resources we have set up in our cloud environment. 
Head into Microsoft Sentinel, under 'Threat Management' select 'Incidents'. 

![img](https://i.imgur.com/SO9VJ9T.png)

I'll go ahead and organize the table by 'Severity' and let's investigate the first incident where the title says "CUSTOM: Brute Force ATTEMPT - Windows".

![img](https://i.imgur.com/o4orRah.png) 

Next, let's establish or assign the owner. assign the status to 'Active' and assign the 'Severity' to 'High'.

![img](https://i.imgur.com/653bdGq.png)

Once those values are set, select "View full details".

Starting with the 'Incident timeline' we can observe when the alerts were triggered that caused the incident to take place. 

![img](https://i.imgur.com/2x2EvTD.png)

Looking into the 'Entities' tab, we'll be able to observe all of the hosts and IPs that correlate with this incident. 

![img](https://i.imgur.com/Gq3Wqrx.png)

If we select one of the IP addresses, we'll be able to analyze it further and observe the geodata that was collected. 

![img](https://i.imgur.com/XhRPmXt.png)

Next, we'll investigate the incident further to get a visualized picture of the underlying scope. To do this, select 'Investigate'. Here, we can look into any suspicious IP entities and see if they are related to any other alerts that were triggered within Microsoft Sentinel. 

![img](https://i.imgur.com/9K9ShUo.png)
