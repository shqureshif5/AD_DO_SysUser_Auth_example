# AD_DO_SysUser_Auth_example
This is an example of how to carryout user auth via AD, so sys-admins can logon to the BIG-IP without a local password. This down not require APM to be licensed

A few pieces of info to highlight, since the info is hard-coded in the JSON
1. 10.1.10.10 is the AD server
2. CN=Users,DC=f5poc,DC=local is where I configured my users - I could have created them in another group
3. In the RemoteAuthRole section, you will note that I set a group BIGIP in AD so that I can accept/deny user access or assign a particular 'role'
4. loginAttribute when using an AD server should be set to sAMAccountName
5. 
