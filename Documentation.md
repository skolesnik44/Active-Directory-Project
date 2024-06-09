# Introduction 

This Active Directory project is an extension of my Packet Tracer project; this domain uses the same ip addressing scheme and departments as my Packet Tracer project 


 ## Security Groups:

I created 3 security groups in this domain: **HR, IT and Marketing**

<img src="https://github.com/skolesnik44/active-directory-project/assets/172089307/49b227d2-32ce-4585-9ea1-4fbee48fc548" width="300" style="height:auto;">

<img src="https://github.com/skolesnik44/active-directory-project/assets/172089307/c960d54f-e357-4a0e-9373-1680ea989982" width="300" style="height:auto;">

<img src="https://github.com/skolesnik44/active-directory-project/assets/172089307/bde58704-663f-43d9-b922-5a9ee7607148" width="300" style="height:auto;">


## Shared Folders:
 
Each group was provided with a dedicated network folder accessible exclusively to its members and administrators


<img src="https://github.com/skolesnik44/active-directory-project/assets/172089307/7364b71c-b890-41b8-903e-95bb7947d042" width="500" style="height:auto;">
<img src="https://github.com/skolesnik44/active-directory-project/assets/172089307/9f205aec-ee56-4bfc-bbe6-c8a7bf13c10c" width="400" style="height:auto;">
<img src="https://github.com/skolesnik44/active-directory-project/assets/172089307/075d5c54-fb18-4803-b4ba-d598b637872f" width="400" style="height:auto;">
<img src="https://github.com/skolesnik44/active-directory-project/assets/172089307/28fd480c-a7a0-4316-9a4c-7c90cee8f9d1" width="400" style="height:auto;">



## Firewall: 

 

I set up two inbound firewall rules: **alloworg** and **denyall**

![captureg](https://github.com/skolesnik44/active-directory-project/assets/172089307/a94b56a4-6b92-4941-8e5d-010f38d65bd3)

 

The rule ‘**alloworg**’ allows inbound connections from the network segments defined in my Packet Tracer project i.e. HR, Marketing, IT, Server Room and Secured Area for Remote Administration 

![Capture](https://github.com/skolesnik44/active-directory-project/assets/172089307/dbf21ce2-bdcb-4f36-9e71-7f05de5c7829)


 

The rule ‘**denyall**’ denies all inbound traffic except from IP addresses defined in ‘alloworg’ due to rule priority 
![Capture2](https://github.com/skolesnik44/active-directory-project/assets/172089307/57fa214e-bec1-42a7-ac2c-fd2cc5bf78ac)

 

 

## Set Default Organization Software: 

 
I made a policy which installs the anti-virus 360TotalSecurity (**for demonstration purposes**) on all computers connected to the domain. Additionally, I have set an option that automatically removes the program from all computers if the policy is removed from Active Directory. 

![Capture2](https://github.com/skolesnik44/active-directory-project/assets/172089307/2708ccc4-4356-4bf5-8b4d-c219ca806400)
![Capture](https://github.com/skolesnik44/active-directory-project/assets/172089307/01506d41-b6be-48e7-8144-03a38ecbf33f)


 

## Password Policy:  

Maximum password age: 90 days 

Minimum password age: 30 days 

Minimum password length: 14 characters 

Number of unique passwords needed before password can be reused: 5 

![passwordpolicy](https://github.com/skolesnik44/active-directory-project/assets/172089307/2e3ee0a7-a430-4980-9f37-9f445cf5a25f)

 

## Account Lockout Policy:  

Lockout duration: 60 minutes 

Max failed logon attempts before lockout: 15 

Failed attempts counter reset: 30 minutes 

![lockoutpolicy](https://github.com/skolesnik44/active-directory-project/assets/172089307/45c4cea6-4bc7-47e2-8a8e-df9c71e84db6)


## Audit Policy 

Audit trail Logons: Enabled 

Audit trail Logoff: Enabled 

Audit trail Account Lockout: Enabled 

![audit](https://github.com/skolesnik44/active-directory-project/assets/172089307/baea047b-9d50-4e4c-8f2c-d8f782c0f6b9)


 

 
