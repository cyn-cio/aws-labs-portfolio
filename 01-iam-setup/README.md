_**Creating IAM Users and Permissions Testing**_

**Objective:**  To show how least-privilege access is enforced.

**AWS Services Used**
- IAM (Identity and Access Management)
- EC2 (Elastic Cloud Compute)

**Steps Performed**
1. Created IAM users: AdminUser, DeveloperUser and ReadOnlyUser
2. Attached permissions to each user: AdministratorAccess for the AdminUser, PowerUserAccess for the DeveloperUser and ReadOnlyAccess for the ReadOnlyUser.
3. Tested permissions for each user: AdminUser can create an EC2 instance, DeveloperUser cannot create an IAM user and ReadOnyUser cannot stop an EC2 user

**Learning Moments**
1. The difference between attaching the permissions to groups versus each user. For learning purposes, it is alright to attach the permissiona to the user directly. This is difficult to track at scale and is not recommended in a working environment. This brings a deeper understanding to the different forms of access control and how they can be utilized when assigning privileges to various users.
2. If configured wrongly, users end up with no access.
3. Permissions should always be verified when a set up is done.
