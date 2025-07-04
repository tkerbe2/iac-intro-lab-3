![tkdev_space_200](https://github.com/user-attachments/assets/31af05be-97b5-4d4e-82ef-4f23203eb7ac)

<br>


# 🧪 HCP Terraform / Terraform Cloud New Account Setup - Guided Lab

In this lab you will setup your brand new HCP Terraform account. If you have not yet created an HCP Account account please do so before starting the steps in this lab. Once the account is created proceed with the steps below.

- [HCP Terraform](https://app.terraform.io/session)

### Resources Created:
This demo creates the following resources:

- An IAM Account
- MFA 
- Custom access portal URL
- Access key and secret key

<br>

# Some Theory 💡

Before getting started lets briefly touch on some high-level information about Terraform Cloud or HCP Terraform. HCP Terraform is a hosted service that allows you to manage your Terraform code, safely store variables, store remote state, and generally collaborate together with other team members. If you recall in our Azure demonstration we deployed some code via Cloud Shell. The state file for that code was local on that Cloud Shell session and when the Cloud Shell session ended, the state file would be deleted. Additionally if we had other team members that wanted to modify our Azure code and change the resources, they would have to do so on that Cloud Shell session, where the state file was stored. With HCP Terraform you can have workspaces where other team members can see exactly what you're doing and contribute to the code as well. 

In HCP Terraform there are a few levels of organization that are important to understand. Firstly, an Organization, this is something you will create immediately and it is the parent object to your projects and workspaces. 

- Projects are like containers to help separate workspaces in a logical way. For example you may have a project that is for a specific set of infrastructure being built and you want all the workspaces that deploy these different pieces of infrastructure, to be organized under one project. 
- By default HCP Terraform has a Default-Project that your workspaces get assigned to. You can also assign variables and variable sets at the project level so that all your workspaces underneath can obtain the variables automatically. 

<br>


> Suggested Reading 📖 
- [What HCP Terraformn](https://developer.hashicorp.com/terraform/cloud-docs)
- [Organizations](https://developer.hashicorp.com/terraform/cloud-docs/users-teams-organizations/organizations)
- [Projects](https://developer.hashicorp.com/terraform/cloud-docs/projects)
- [Workspaces](https://developer.hashicorp.com/terraform/cloud-docs/workspaces)


<br>

# Lab Steps

### 1. Log into HCP Terraform

- Log into the portal and you should have no organizations. In this example I have one created already.

![image](https://github.com/user-attachments/assets/45460ac9-8c0e-4658-ad36-753b9550d7ef)


<br>

***

### 2. Create an organization

- You should immediately be presented the option to create a new organization.
- An organization is the highest level object in HCP Terraform.

  -- Organization 
    -- Workspace
![image](https://github.com/user-attachments/assets/3e7d5deb-799d-4ee3-9f56-83ea6d98c9c6)







# ✨ Congratulations!

***

You've finished this lab and have completed the following items:
- ✅ Created a new AWS account.
- ✅ Logged into your AWS root account.
- ✅ Created an AWS IAM user that will be used for Terraform.
- ✅ Created an access key and secret key with the new user.

***

