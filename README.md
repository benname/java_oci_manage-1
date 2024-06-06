# <p align="left">R-Bot⭐</p>
<p align="left">
  <a href="https://t.me/apchyo"><img src="https://img.shields.io/static/v1?label=%E7%BE%A4%E7%BB%84&message=telegram&color=brightgreen"/></a>
  <a href="https://t.me/agentONE_R"><img src="https://img.shields.io/static/v1?label=%E9%A2%91%E9%81%93&message=telegram&color=blueviolet"/></a>
  <a href="https://t.me/radiance_helper_bot"><img src="https://img.shields.io/static/v1?label=%E6%9C%BA%E5%99%A8%E4%BA%BA&message=telegram&color=red"/></a>
 <img src="https://img.shields.io/github/stars/semicons/java_oci_manage.svg?style=flat-square&label=Stars&logo=github"/>
</p>

### Preface
> The system is currently used for some quick operations on Oracle Cloud/Azure Cloud.
> 
### Declaration
> 
> The system is dual-ended, and the robot does not store any sensitive data.
> 
> The API private key is local on your client server, driven by the bot to operate your client. You can terminate the service at any time.
> 
> If you mind, please do not use it. Thank you.
>
> Disclaimer
> 
> Any scripts involved in the projects released by this repository are only for testing and research purposes, and are prohibited for commercial use. Their legality, accuracy, completeness, and effectiveness cannot be guaranteed. Users should judge according to their circumstances.
>
> All users must comply with laws and regulations when using any part of the project. Users must bear all consequences of misuse. We are not responsible for any issues with the scripts, including but not limited to any losses or damages caused by script errors.
>
> If any entity or individual believes that the project may infringe on their rights, they should notify us promptly and provide proof of identity and ownership. We will delete the relevant files upon receiving verification documents.
>
> Anyone who views this project in any way or directly or indirectly uses any scripts from this project should read this disclaimer carefully. I reserve the right to change or supplement this disclaimer at any time. By using and copying any related script or rules of this project, you are deemed to have accepted this disclaimer.
>
> You must completely delete the above content from your computer or mobile phone within 24 hours after downloading.
>
> If you use or copy any scripts made by me from this repository, you are deemed to have 'accepted' this disclaimer. Please read carefully.
### Bot Usage Process

- 【First】Please follow [the channel](https://t.me/agentONE_R) and [the bot](https://t.me/radiance_helper_bot)

- 【Then】[Install and configure ](https://github.com/semicons/java_oci_manage/blob/main/md/install.md)(you can choose between public network mode and local non-public network mode)

- 【Next】Use the bot command '/raninfo' to generate random information, then insert it into the 'client_config' file (created after executing the one-click installation command), and also input the Oracle Cloud API parameters into the configuration file (or upload API parameters via the bot).

- 【Finally】 Restart the bot by running bash sh_client_bot.sh, and you can start using the bot!

> ps:The program comes with the feature to open port 9527. If the port is not open, you can manually enable it. You can test whether the port is open by visiting this test website(https://port.ping.pe).
>
> ps:If you use the local mode, there is no need to open any ports.
> 
> ps:The script supports passing arguments. You can change the default port 9527 to another port by using the command 'bash sh_client_bot.sh 8888', where 8888 is the new port number you want to use.

### Uninstall
```bash
rm -rf gz_client_bot.tar.gz client_config r_client.jar sh_client_bot.sh log_r_client.log debug-*.log
```
If JDK is not required, it can also be uninstalled:
```bash 
apt remove openjdk*
```

### Documentation and Help
- [Implemented Features](https://github.com/semicons/java_oci_manage/blob/main/md/function.md)

- [Robot Operations and Command Guide](https://github.com/semicons/java_oci_manage/blob/main/md/BOT-README.md)

- [Oracle Cloud API Parameter Retrieval and Upload(tip：When creating an API file for flashing devices only, you can restrict various operational permissions.)](https://github.com/semicons/java_oci_manage/blob/main/md/oracle.md)

- [Azure API Parameter Retrieval and Upload](https://github.com/semicons/java_oci_manage/blob/main/md/azure.md)

- [Frequently Asked Questions](https://t.me/agentONE_R/41)



### Changelog
<details>
<summary>examine Releases explain</summary>
 
> Proof that the Project is Still Active


</details>
