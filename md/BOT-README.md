> Robot Usage Guide

# Contents

- [1.Robot Command Menu Explanation](#1Robot Command Menu Explanation)
- [2./oracle Keyboard Menu Explanation](#2oracle Keyboard Menu Explanation)


## 1.Robot Command Menu

### /oracle

- Access the Oracle Cloud operation keyboard for actions such as starting machines, etc.

### /azure

- Access the Azure Cloud operation keyboard for actions such as starting machines, etc.

### /me

- Retrieve personal lightning subscription information

### /raninfo

- Generates or resets to random user information

Please save this information. If you encounter issues such as being blocked on Telegram, you can use this information to rebind your Telegram account.

### /qrcode

- Lightning Access Recharge

Obtain a QR code for payments, used for donations or purchasing Lightning Access. After payment, you will receive an activation code to activate the Lightning Access.

### /codeflash

- Activate Lightning Access without a payment note

If you did not include a note with your payment, you can activate your Lightning Access by using this command with your transaction order number. Usage: /codeflash transaction_order_number.

### /flash

- Compare standard access and Lightning Access

### /migrate

- Transfer Lightning Access

Transfer your Lightning Access to your current login account. Use /migrate old_username old_password.  

### /oci

- Upload Oracle or Azure configurations

Upload your current client configuration details here. For security reasons, if you're uploading Oracle configurations, the key_file must be uploaded to your client server directly. Only specify the path to your private key here.

### /getflash

- Activate Lightning Access with an activation code

To activate your Lightning Access, use /getflash activation_code.

### /command

- Execute shell commands on the current client

Allows you to execute shell commands on your current client server.

### /pubkey

- Add an SSH public key required for booting.

### /oproxy

- Add a proxy to a client profile.

Use this command to add an HTTP proxy to a specific client profile, allowing requests to be made without using the client's IP.

### /clearlock

- Clear locks caused by too many incorrect password attempts.

### /qb

- Address issues with recharge not being credited or provide feedback on advertising partnerships.

### /qs

- Dedicated support line for Lightning users

Prevents lockouts caused by brute force attacks on your information.

### Do not operate without admin rights

## 2.Oracle Keyboard Menu

### 1. Boot (ARM-specific)

You can boot your account with custom system configurations and CPU types, but you need to know Oracle's internal names for these. The delay is measured in seconds. It's important to note that booting requires a confirmation—only after clicking the keyboard's confirm button again does the boot process start.

### 2. IP Management

IP Replacement: You can change the IP.
Assign to Cloudflare Managed Domain: Quickly assign the machine IP to a domain managed by Cloudflare.
Pseudo-DDNS Function: While changing the IP, you can also update the DNS records of the domain bound to the IP, achieving a pseudo-DDNS functionality. (This requires pre-entering Cloudflare's email and key in the configuration file. Obtain the Cloudflare key from My Profile -> API Tokens -> API Keys -> Global API Key.)
Delete Domain: Removes all domains associated with the current IP.
Delete Current IP: You can delete the current IP.

### 3.Boot from Suspension

This function allows you to boot the machine from a shutdown state without needing to delete the disk and reboot.

### 4. IPv6 Management

Current accounts can perform actions such as changing IPv6 addresses.

### 5. Instance Upgrading/Downgrading

Current accounts can upgrade or downgrade CPU and memory specifications on Oracle machines.

### 6. Instance Management

In instance management, current accounts can delete instances, attach additional IPv4 and IPv6 addresses, intelligently attach reserved IPs, disable or enable Oracle's monitoring, forcibly restart, modify instance names, delete all IPv6 addresses, and reset the system to its initial setup.

### 7. Disk Management

Current accounts can delete the boot disk, increase its capacity (but not decrease it), detach and attach the boot disk, and maximize Oracle VPU performance to enhance IO speed.

### 8. Cloud Account Management

Current accounts can add administrative users and upload APIs, reset current user passwords, query user emails in bulk, and delete users.

### 9.  Instance Status Monitoring Notification

Once enabled, it monitors the status of all instances regularly and notifies you of any anomalies.

### 10. Instance Status Monitoring Auto-Restart

When enabled, it automatically monitors all instances and attempts to restart them if any anomalies are detected.

### 11. Open Cloud Panel Ports

With one click, open all cloud panel ports for the current account and clear the account's firewall rules (not instance firewalls, but the main firewall managed by Oracle).

### 12. Oracle Workflow Errors

Only queries the errors returned by the last three Oracle workflow operations.

### 13. Profile Management

If multiple profiles, i.e., multiple configuration files, are filled in the client, you can switch and select different configurations here or delete profiles that are not needed.

### 14. Client Management

If you have multiple machines running the script, you can switch between different clients and configurations here, and delete any clients that are not needed.

### 15. One-Click Testing

Performs a batch one-click activity test for all profiles and all client accounts.

### 16. Monitoring (Automatic IP Change)

Set up monitoring for a specified IP on the current client to trigger an IP change and domain binding. Choose the IP, decide if a proxy is needed (without a proxy, the current client IP is used for assessment), and perform checks like Netflix non-original series detection.

### 17. Quick Boot

Save boot configurations and then boot multiple configurations and profiles simultaneously, or boot multiple configurations across different clients at the same time (if both multiple profiles and clients are selected, only the multiple clients booting simultaneously will take effect).

### 18. Oracle Subscription Info

Check the current account's Oracle free subscription dates and amounts.

### 19. Monthly Data Usage

View the data usage for the current account.

### 20. Query Quotas

Check your quotas for Oracle Cloud instances, network, and storage.

### 21. View Running Tasks

Query all tasks currently running on clients, such as booting and upgrading.

### 22. View Client Load

Check the current load on the client.

### 23. Occupy 25% Memory

Intelligently increase the program's memory usage to 25%; if the system's current usage is below this, it will adjust accordingly. If already at 25%, it will not increase further.

### 24. Clear Cache and Usage

Clear the system memory's cache and the 25% usage allocation.

### 25. View Monthly Expenditure

View spending details and amounts for paid accounts; for multi-region accounts, these need to be checked from the main account.

### 26. Clear All 2FA Devices

Remove all bound two-factor authentication devices (useful if a device is lost or the keys are misplaced).

### 27. Restart Client

Restart the current client.

### 28. Upgrade Client

Check all clients and upgrade them if necessary (if an upgrade is detected, all operations will be interrupted).

### 29. Disable Locked Accounts with One Click

Check all clients for any locked accounts and comment them out (configurations will not be deleted).

### 30. Disable and Delete API of Locked Accounts

This operation permanently deactivates the API after deletion; if you need to use it again, you must regenerate the API file from the official website (if you've lost access to your current account's email or can't log in, and only have the current API, this means you will lose your valuable account).

### 31. Query Latest Logs

Query Latest Logs.
