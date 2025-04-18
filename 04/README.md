# Section 04 : Identity Access Management
## Lesson 15 : Users, Groups, Policies

Identity Access Management is a global service.

Do not use your root account. Create an admin account. Create users and groups for their job functions. 

Groups can only contain Users - not other groups.  
Users can belong to multiple groups. Users do not have to belong to a group, but thats not best practice.  

Users and Groups can be assigned JSON documents called policies. These desine the permissions for the usere. Apply the concept of *least privilege principle* - dont give the user more permissions than they need.  

## Lesson 16 : Users, Groups Hands On 

Hands on excercise is done through the console. :P  

Create user, click the checkbox for console access. Click Auto-generate password and User must change password at sign-in check boxes.   

Check Add user to group, then click Create group.We will create an ADMIN group. Check the AdministratorAccess group. Click *create user group*.  

Add the user to the admin group and click Next.  

The review screen will now display. Click *Create User* to add the user.  

## Lesson 17 : IAM Policies

Attaching policies at a group level, these policies are attached to all users in that group.

IAM Policies Structure: Version, ID, Statement ( SID, Effect, Principal, Action, Resource) 

## Lesson 18 : IAM Policies Hands On

Hands on excercise is done through the console. :
P 

## Lesson 19 : IAM MFA Overview

Password policy : Sronger the password, the higher the security.  

Multifactor Authentication : password you know and a security device you own. Google Authenticator, Authy, standalone hardware device such as a YubiKey.  

## Lesson 20 : IAM MFA Hands On

Hands on excercise is done through the console. :
P

Account Settings : Set a password policy.  

## Lesson 21 : Access Keys, CLI, SDK

Hands on excercise is done through the console. :
P

AWS CLI: shell access to AWS. 

AWS SDK: Language specific APIs.
- Allows access and management of AWS services programmatically.  
- Can be imbedded in your application
- Supports multiple SDKs, Mobile SDKs, and IoT Device SDKs.  

BOTO is Python.  

## Lesson 22 : CLI Windows

Skipped as I do not have Windows. 

## Lesson 23 : CLI Mac

```brew install awscli```

## Lesson 24 : CLI Linux

Skipped as I do not have a current Linux device for AWS purposes.

## Lesson 25 : CLI Hands On

Create an access key. 

> aws configure
- Add Access Key ID  
- Add AWS Secret Key  
- Add Default region name  
- Set Default output format

## Lesson 26 : Cloudshell

I prefer AWS CLI. I'm not sure I would ever use this.  

Author says cloudshell is not necessary or required for this class.

## Lesson 27 : IAM Roles for Services

Some AWS services will need to preform actions on your behalf such as EC2, Lambda or Cloudformation.  

## Lesson 28 : IAM Roles Hands On

Create an IAM role for EC2. Assign it the IAMReadOnly policy. We will use this in future lessons.  
## Lesson 29 : IAM Security Tools

IAM Credentials Report exists at the account level. Whereas IAM Access Advisor exists at the user-level.

## Lesson 30 : IAM Security Tool Hands On

IAM > Credentials Report. Download the CSV.  

IAM > Users > specific user > Last Access Tab.  

## Lesson 31 : IAM Best Practices

- Do not use the root account, use your user account.  
- One physical user == One AWS user.  
- Assign users to groups, assign permissions to groups.  
- Create a strong password policy.  
- Use and enforce MFA.  
- Create roles for AWS services.  
- Use Access Keys for CLI/SDK.  
- Audit permissions.
- Never share users or keys.  

## Lesson 32 : Shared Responsibility IAM

AWS is responsible for : Infrastructure, Global network security, Configuration, Vulerability analysis, Compliance validation.

Admins are respnsible for : Users, Groups, Roles, Policy management, Monitorng, MFA, Key rotation, IAM tools and permissions, Access patterns.  

## Lesson 33 : IAM Summary

- IAM Users : mapped to a physical user, has a password.  
- Groups : contain users only.  
- Policies : JSON document that defines permissions for groups applied to users.  
- Roles : defined for AWS services.  
- Security : MFA & password policy.  
- CLI : Manages your services from the command line.  
- SDK Manages your services using a programming language.  
- Access Keys : AWS access from CLI/SDK.  
- Audit : IAM Credentials Report / IAM Access Advisor.  

## Quiz : IAM Quiz 

Read the questions carefully.
