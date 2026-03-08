# Windows-VM-Security-Hardening

### 1. Update Windows fully
  - Settings -> Update & Security

  
### 3. Enable Windows Defender:
  - Turn on  Real- time protecton
  
  - Turn on cloud protection

  
### 4. Local Policy Hardening
  - Type **Run** into the search window and type `secpol.msc`
  - Click **Account Policies**
    - Set password complexity
    - 12-char minimum
    - 365-day max age


    
### 5. Firewall:
  - Block inbound RDP(3389) except localhost
    - Enable Logging


  
### 6. Disable SMBv1:
  - PowerShell

   *` Disable-WindowsOptionalFeature-Online-FeatureName SMB1Protocol`*  
