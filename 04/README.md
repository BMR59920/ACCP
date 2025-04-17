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

## Lesson 22 : CLI Windows

## Lesson 23 : CLI Mac

## Lesson 24 : CLI Linux

## Lesson 25 : CLI Hands On

## Lesson 26 : Cloudshell

## Lesson 27 : IAM Roles for Services

## Lesson 28 : IAM Roles Hands On

## Lesson 29 : IAM Security Tools

## Lesson 30 : IAM Security Tool Hands On

## Lesson 31 : IAM Best Practices

## Lesson 32 : Shared Responsibility IAM

## Lesson 33 : IAM Summary

## Quiz : IAM Quiz 

