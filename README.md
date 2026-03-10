# ‼️ Windows-VM-Security-Hardening

## 1. Update Windows Completely
  - Settings -> Update & Security

  
## 2. Enable Windows Defender:
  - Turn on  Real- time protecton
  - Turn on cloud protection

<img width="600" height="500" alt="Windows11-VM" src="https://github.com/chosn12/Windows-VM-Security-Best-Practices/blob/358825bdcf5b374bc7f5ae86563976f0bbd88fbe/doc/screenshots/Enable%20Defender.png"/>


  
## 3. Local Policy Hardening
  - Type **Run** into the search window and type `secpol.msc`
  - Click **Account Policies** then **Password Policy**
    - **Enable** password complexity
    - Set password length to **12-char minimum**
    - Set maximum password age to **365-day max age**


<img width="600" height="500" alt="Windows11-VM" src="https://github.com/chosn12/Windows-VM-Security-Best-Practices/blob/a6ac530be79de1dea876e90391ab9924c7f6634a/doc/screenshots/Local%20Policy%20Hardening.png"/>

    
## 4. Firewall:
  - Block inbound RDP(3389) except localhost
    - Enable Logging


  
## 5. Disable SMBv1:
  - PowerShell

   *` Disable-WindowsOptionalFeature-Online-FeatureName SMB1Protocol`* 

This command displays the status of SMB1.


<img width="600" height="500" alt="Windows11-VM" src="https://github.com/chosn12/Windows-VM-Security-Best-Practices/blob/9522059e32275001a9ba6ef187838b46bb326860/doc/screenshots/SMB1%20Status.png"/>



## 6. Policy Export
  - cmd

    *` gpresult /user UserA /scope computer /r `*
    
<img width="600" height="500" alt="Windows11-VM" src="https://github.com/chosn12/Windows-VM-Security-Best-Practices/blob/20479762a72b27f0f9777f44701b4387ca56cd49/doc/screenshots/Policy%20Export.png"/>

     
