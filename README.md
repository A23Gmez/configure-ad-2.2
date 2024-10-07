# Configuring-AD Part 2.2

<h1>Group Policy and Managing Accounts</h1>

![image](https://github.com/user-attachments/assets/3b32e7e9-8b18-4233-8a94-dde8afc44543)

<h3>Dealing with Account Lockouts</h3>

![image](https://github.com/user-attachments/assets/b94e9a0e-74e0-4306-934b-f9fd7ec87764)
![image](https://github.com/user-attachments/assets/4262f2a1-46cb-4981-9375-6b9283f4b68e)
![image](https://github.com/user-attachments/assets/7bf7ae08-216a-425f-bfbe-85669e7faf9c)
- Logged into dc-1.
- Edit Domain Policy to Lock out Users exceed 5 attempts.
- Execute gpupdate /force on my Jane_Admin account, to update group policy password changes to my domain. 

![image](https://github.com/user-attachments/assets/dbe9414a-f5e5-4687-b1e4-a811e8517061)
- confirmed the group policy changes using gpresult /r.

![image](https://github.com/user-attachments/assets/b008f6a0-5f00-4012-a79b-ecb7751b5e19)
- Pick a random user account I created previously.
- Attempt to log in with it 6 times with a bad password.
- Comfirmed Group Policy password change Lockout after 5 attempts.


![image](https://github.com/user-attachments/assets/ceab25a4-c3d3-4654-9ecf-eff657f44e75)
- Observe that the account has been locked out within Active Directory.

![image](https://github.com/user-attachments/assets/e2271e45-3ff2-418c-852e-acee7bf1c361)
- Unlock the account
- Reset the password

![image](https://github.com/user-attachments/assets/37f818cc-a056-446e-9f8d-705612853192)
- Attempt to login/confirmed login

<h3>Enabling and Disabling Accounts</h3>
- Disable the same account in Active Directory
- Attempt to login with it, observe the error message
- Re-enable the account and attempt to login with it.

<h3>Observing Logs</h3>
- Observe the logs in the Domain Controller
- Observe the logs on the client Machine
- Precursor to cybersecurity and security operations: joshmadakor.tech/cyber



