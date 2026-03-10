# ‼️ Windows-VM-Security-Hardening

## 1. Update Windows Completely
  - Settings -> Update & Security

  
## 2. Enable Windows Defender:
  - Turn on  Real- time protecton
  - Turn on cloud protection

<img width="800" height="500" alt="Windows11-VM" src="https://github.com/chosn12/Windows-VM-Security-Best-Practices/blob/358825bdcf5b374bc7f5ae86563976f0bbd88fbe/doc/screenshots/Enable%20Defender.png"/>


  
## 3. Local Policy Hardening
  - Type **Run** into the search window and type `secpol.msc`
  - Click **Account Policies**
    - Set password complexity
    - 12-char minimum
    - 365-day max age


<img width="700" height="500" alt="Windows11-VM" src="https://github.com/chosn12/Windows-VM-Security-Best-Practices/blob/a6ac530be79de1dea876e90391ab9924c7f6634a/doc/screenshots/Local%20Policy%20Hardening.png"/>

    
## 4. Firewall:
  - Block inbound RDP(3389) except localhost
    - Enable Logging


  
## 5. Disable SMBv1:
  - PowerShell

   *` Disable-WindowsOptionalFeature-Online-FeatureName SMB1Protocol`*  

   <img width="800" height="500" alt="Windows11-VM" src="https://github.com/chosn12/Windows-VM-Security-Best-Practices/blob/9522059e32275001a9ba6ef187838b46bb326860/doc/screenshots/SMB1%20Status.png"/>


## 6. Policy Export
  - cmd

    *` gpresult /h report.html`*

     <img width="800" height="500" alt="Windows11-VM" src=""/>
