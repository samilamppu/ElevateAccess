This repo contains Azure Logic App (Azure Sentinel Playbook) sample for ingesting Cloud App Security activity log to Azure Sentinel. Logic App name is Ingest-MCAS-Activity-Log-Data but can be changed when needed.

## Warning
More detailed planning is needed in the production instance for Logic Apps to handle data pulled from Cloud App Security API. This is just a sample to get started.

## Deployment
Copy Logic Apps as a raw and implement it as a code view in Azure Logic Apps. The following modifications are needed:

* **Line 39** - insert tenant name
* **Line 54** - insert MCAS API token
You need to add API connnection details based on your environment to Log Analytics connection details

![image](https://user-images.githubusercontent.com/18166822/107668629-8b6e7480-6c99-11eb-942f-5579ca3141b0.png)

**Note!** API connection to the Log Analytics needs to be defined.
