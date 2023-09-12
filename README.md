# Azure-Cloud-Security-Hardening

## Introduction
In my Azure SOC Lab, both the Windows VM and Linux VM where receiving large volumes of malicious activity such as password brute force attempts on Azure AD, Microsoft SQL server and Linux SSH server as well as DDOS attacks. This was due to impromperly configured security settings, which were exposing the virtual machines to the public internet, allowing traffic from any IP Address on any port. Using the NIST 800-53 Security Controls framework, I was able to reduce the amount of malicious traffic affecting my Azure Cloud environment by 95%.

## Applying NIST 800-53 Security Controls
The control from NIST 800-53 that deals whith securing network endpoints is Section SC-7: Boundary Protection.<br>
<br>
The information system:<br>
a. Monitors and controls communications at the external boundary of the system and at key internal boundaries within the system; <br>
b. Implements subnetworks for publicly accessible system components that are [Selection: physically; logically] separated from internal organizational networks; and <br>
c. Connects to external networks or information systems only through managed interfaces consisting of boundary protection devices arranged in accordance with an organizational security architecture. <br>
<br>
Specifically, section SC-7(3) states:<br>
"The organization limits the number of external network connections to the information system. Limiting the number of external network connections facilitates more comprehensive monitoring of inbound and outbound communications traffic."<br>
<br>
Azure's Microsoft Defender for Cloud gave me the following recommendations for security controls based on NIST 800-53 SC-7(3):

![Screenshot 2023-09-07 190615](https://github.com/Lachiecodes/Azure-Cloud-Security-Hardening/assets/138475757/88345ec8-e132-42e4-a080-a21c8dca21e6)

## Configuring and Hardening Network Security Groups
![Screenshot 2023-09-07 200607](https://github.com/Lachiecodes/Azure-Cloud-Security-Hardening/assets/138475757/6fe25e75-d941-45a2-8deb-8582030414d5)

![Screenshot 2023-09-07 200646](https://github.com/Lachiecodes/Azure-Cloud-Security-Hardening/assets/138475757/d8b2d8ca-3f49-42a4-8226-8f228d98704b)

## Configuring Private Endpoint Access to Azure Key Vault and Blob Storage


## Enabling Firewall on Azure Key Vault 


## Conclusion


