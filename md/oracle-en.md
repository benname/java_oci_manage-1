### Retrieving API Parameters for Oracle Cloud
```text
【Navigation Options, any method is acceptable】(tips: If you want to limit permissions for device flashing, it's recommended to create a user with only instance management permissions and extract the API for flashing operations, thus limiting the API to creating instances and similar permissions)

- 1.In English interface, directly search for "domain", find "Domains" under Services, select your default "Default", click on "Users" on the left, select your user, and add API keys at the bottom left.


- 2.If you don't have user settings, search for "user" (switch to Chinese language), select a username, then API Keys >> Add API Key -> (check the parameters at the three dots next to the fingerprint).


- 3.If unsure how to search, click on the left menu bar, navigate to Identity and Security => Users => select a username => API Keys >> Add API Key -> (check the parameters at the three dots next to the fingerprint).


- 4.Oracle backend => User Settings >> Resources >> API Keys >> Add API Key -> (check the parameters at the three dots next to the fingerprint).
- Note: These configurations are essential for connecting to the Oracle Cloud interface.

The format is roughly as follows↓
[DEFAULT]
user=ocid1.user.oc1..aaaaaaaaxxxxgwlg3xuzwgsaazxtzbozqq
fingerprint=b8:33:6f:xxxx:45:43:33
tenancy=ocid1.tenancy.oc1..aaaaaaaaxxx7x7h4ya
region=ap-singapore-1
key_file=Specify the path to your API key file like so:/root/rbot/xxx.pem

Uploading via Bot: /oci [DEFAULT]
user=ocid1.user.oc1..aaaaaaaaxxxxgwlg3xuzwgsaazxtzbozqq
fingerprint=b8:33:6f:xxxx:45:43:33
tenancy=ocid1.tenancy.oc1..aaaaaaaaxxx7x7h4ya
region=ap-singapore-1
key_file=/root/rbot/xxx.pem
```
- Insert the parameters from the API key configuration preview in Oracle user settings into the client_config file. Please ensure the private key file path is correct. The private key file is generated and downloaded or uploaded when you add the API key. Place it in your desired location, such as:
- key_file=/root/oci/oci_api_key.pem)
- ![image](https://github.com/semicons/java_oci_manage/blob/main/1646021119866.jpg)
