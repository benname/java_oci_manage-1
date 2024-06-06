### Azure Cloud API Parameter Retrieval and Configuration Upload
```text
1. Log in to the Azure portal and select the Cloud Shell icon in the upper right corner.
2. Choose PowerShell and execute the following commands to retrieve API-related parameters.
az ad sp create-for-rbac --role contributor --scopes /subscriptions/$(az account list --query [].id -o tsv)
3. Use the /oci command to directly upload your configuration. Example:
  /oci {
  "appId": "xxxxx-xxx-xx-xxx-xxxx",
  "displayName": "azure-cli-11111-12-111-11-222-22",
  "password": "xxxxx~oxjTxxxxxxxxb_I",
  "tenant": "xxxx-xxxx-xxxx-xxxx-xxxxxxxx"
  }
```
![image](https://github.com/semicons/java_oci_manage/blob/main/az.jpg)
