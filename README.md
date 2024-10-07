# Configuring-AD Part 2.2

<h1>Group Policy and Managing Accounts</h1>

![image](https://github.com/user-attachments/assets/3b32e7e9-8b18-4233-8a94-dde8afc44543)

<h3>Dealing with Account Lockouts</h3>
Get logged into dc-1
Pick a random user account you created previously
Attempt to log in with it 10 times with a bad password

Configure Group Policy to Lockout the account after 5 attempts:
How To Configure Account Lockout Threshold in Group Policy

Attempt to log in with it 6 times with a bad password

Observe that the account has been locked out within Active Directory
Unlock the account
Reset the password
Attempt to login with it

Enabling and Disabling Accounts
Disable the same account in Active Directory
Attempt to login with it, observe the error message
Re-enable the account and attempt to login with it.

Observing Logs
Observe the logs in the Domain Controller
Observe the logs on the client Machine
Precursor to cybersecurity and security operations: joshmadakor.tech/cyber

Finish the lab, but do not delete the VMs in Azure. We will use them for upcoming labs.
If you are done for the day and want to save money, simply “Stop”/turn off the VMs within the Azure Portal

