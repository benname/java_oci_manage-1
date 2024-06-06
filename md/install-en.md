#### 1.Linux One-Click Install/Update (Use 'bash sh_java_oci.sh' after completion to restart)
- The script does not create a directory. You can manually create one for easier management. For example: mkdir rbot && cd rbot
```bash
wget -O gz_client_bot.tar.gz  https://github.com/semicons/java_oci_manage/releases/latest/download/gz_client_bot.tar.gz && tar -zxvf gz_client_bot.tar.gz --exclude=client_config  && tar -zxvf gz_client_bot.tar.gz --skip-old-files client_config && chmod +x sh_client_bot.sh && bash sh_client_bot.sh
```
#### 2. Modify Configuration File Parameters
- Edit the client_config file according to the parameter instructions. For instance, set model to local to initiate local mode without a public IP.
```text
#Place your API configuration details between oci=begin and oci=end within the client_config file. This setup supports multiple configuration files, and you can switch between different operational accounts using the robot's profile management feature.
oci=begin

[DEFAULT]
user=ocid1.user.oc1..aaaaaaaaxxxxgwlg3xuzwgsaazxtzbozqq
fingerprint=b8:33:6f:xxxx:45:43:33
tenancy=ocid1.tenancy.oc1..aaaaaaaaxxx7x7h4ya
region=ap-singapore-1
key_file=Specify the path to your API key file like so:/root/rbot/xxx.pem

[tokyo]
user=ocid1.user.oc1..aaaaaaaaxxxxgwlg3xuzwgsaazxtzbozqq
fingerprint=b8:33:6f:xxxx:45:43:33
tenancy=ocid1.tenancy.oc1..aaaaaaaaxxx7x7h4ya
region=ap-singapore-1
key_file=Specify the path to your API key file like so:/root/rbot/xxx.pem

oci=end



#User Information: Configure from https://t.me/radiance_helper_bot (the bot can generate random information using the /raninfo command)
#Required
username=
#Required
password=


#Cloudflare Functionality Parameters (optional)
# Optional: Cloudflare email
cf_email=
# Optional: Cloudflare key, obtainable from My Profile -> API Tokens -> API Keys -> Global API Key
cf_account_key=


#Optional: Local machine IP and port number (advanced users can also specify a domain name). If not specified, the system will automatically obtain the local IP and use the default port 9527. It's recommended that novice users leave this blank. If specified, the format should be: https://xxx.xx:9527
local_address=
#Optional: URL name (default is "address" but can be changed in the bot settings)
local_url_name=

#Optional: Startup mode. Set to 'local' to initiate in local mode without a public IP (internet connection is required). Leave blank or fill in another value to start in port mode.
model=



#Place your Azure API configuration information between azure=begin and azure=end. This setup supports multiple configuration files, allowing you to switch operational configurations using the bot's profile management feature. You can upload configurations in the original format ({"appId":"xxx", "password":"xxx", ...}).
azure=begin

[az001]
appId=551xxxx7-xxxx-xxxx-xxxx-b9xxxx60cc65
password=T618Q~.LIy_xxxxx~jm~xxxxxx
tenant=xxxx3713-xxxx-4cb5-xxxx-3001060xxxxx

azure=end
```

#### 3. Start, Terminate, View Logs, Uninstall
```text
Please enter the required parameters in the configuration file first, then execute the necessary command below:

To start or restart:
bash sh_client_bot.sh 

To view logs (press ctrl + c to exit logs):
tail -f log_r_client.log  

To terminate the program:
ps -ef | grep r_client.jar | grep -v grep | awk '{print $2}' | xargs kill -9  

To uninstall the program:
rm -rf gz_client_bot.tar.gz client_config r_client.jar sh_client_bot.sh log_r_client.log debug-.log 
If JDK is also no longer needed, it can be uninstalled with:apt-get remove openjdk*

```
