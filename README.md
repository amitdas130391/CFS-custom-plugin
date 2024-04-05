Copilot for Security Plugin to run a Dynamic KQL Query to estimate Microsoft Sentinel Costs for a specific time and date range by running a KQL query against the Usage table in Microsoft Sentinel.

		
	Pre-requisites
1.Copilot for Security Enabled.
2.Access to upload custom plugins.
3.Microsoft Sentinel Workspace created.
4.Parameters for KQL Plugin - Microsoft Sentinel Workspace Name, Subscription ID, Resource Group Name and Entra Tenant ID.

		Instructions

	Upload the Custom Plugin
1.Obtain the file KQL-Sentinel-SentinelCost.yaml from this directory.
2. Modify the yaml file to specify your specific Entra TentantId, SubscriptionId, ResourceGroupName and WorkspaceName for your Sentinel instance. You can also modify the KQL query at the bottom of the plugin to adjust your specific $ Per GB rate for Sentinel data ingestion (size * 4.3).

![image](https://github.com/amitdas130391/CFS-custom-plugin/assets/83881948/2e06ac42-ffd7-40b0-b883-2c83f3727cfd)

3.Upload the custom plugin and verify it's activated.

![image](https://github.com/amitdas130391/CFS-custom-plugin/assets/83881948/8bb4fc42-37f2-4c7b-a9d6-cfafb9afc6ce)

		Plugin Utilization
Here's some sample queries you can utilize to trigger this plugin - Always include a time and date range.

Can you lookup what my Sentinel costs were in the past 7 days?
Can you provide me a summary of my total Sentinel costs between March 1, 2024 and March 15, 2024?

![image](https://github.com/amitdas130391/CFS-custom-plugin/assets/83881948/9f15566c-9638-4623-bb31-47eaec86a0ff)


