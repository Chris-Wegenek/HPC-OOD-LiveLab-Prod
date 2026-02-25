# Lab 2: Logging into the HPC Application

## Introduction

In this lab you will log into the Open on Demand application creatred by the terraform stack using the domain that was created. This will give you access to all of the HPC servers created and alow you to use the application to manage them.

**Estimated Time:** 15 Minutes


### Prerequisites

It is assumed that you:

- The ability to access resources in your tenancy.
- Have already created and deployed a stack successfully, and have not manually deleted any components that were created.
- You have entered your email in Lab 1, Task 2, Step 14.


### Objectives

In this lab, you will:

- Access the activate profile email.
- Configure the domain.
- Access the HPC management application, "Open On Demand (OOD)."

## Task 1: Find the activate profile email

While the stack successfully deployed and created the domain, a welcome email should have been sent to the email you entered in Lab 1, Task 2, Step 14.

``Note: if you used a preexisting Domain then you can skip this task.``

### 1. Find the email

Log into your email and find the "Activate your profile in account..." email.

Click the "**Activate Your Account**" button.

Then reset your password and return to the OCI dashboard for the next step.

![photo of email](./images/activate_profile.png)

## Task 2.  Configure the Domain

### 1. First log in to your OCI console and select the hamburger dropdown menu.

![Hamburger Menu](./images/hamburger.png)

Then use the search bar to look up "**Domains**"

Click on "**Domains**" with "Identity" after it

![image](./images/domains.png)

### 2. Select your domain

Make sure you have the **compartment** where you created the domain.

Then once you see your domain click on its name in the blue text.

![OOD Domain and compartment screen](./images/domain-compartment-select.png)

### 3. Open the integrated application

From the main domain details screen select the integrated applications tab.

![OOD Domain main screen](./images/main_domain_screen.png)

Then from there select the name of your integrated application in blue text.

![OOD Domain integrated applications screen](./images/domain_integrated_applications.png)

### 4. Select Oath configuration and fill in the details

From the details screen of your integrated application select the "**Oath configuration**" tab.

Then click on the "**Edit Oauth configuration**" button near the top.

![Integrated applications and Oauth configuration](./images/integrated_applications_oath.png)

Next you will need to scroll down to the bottom of the popup menu and switch on the "**Add app roles**."

Then click the black "**Add app roles**." button.

![Where to add app roles](./images/add_app_roles.png)

Then you want to seach and add roles for:
   
```
<copy>Me<copy></copy>
```
```
<copy>Identity Domain Administrator<copy></copy>
```
```
<copy>Signin<copy></copy>
```
Then click the black "**Add**." button in the bottom right.

![Screen where you lookup roles](./images/role_lookup.png)

Once you are back to the previous screen you can click submit.

![What the added roles look like](./images/finalized_added_roles.png)

### 5. Log into the application

Log in to your user profile using the Post-logout redirect URL link.

To log in you will use your ood user name and ood password you entered in Lab 1: Task 2, Step 14. 

![Log in link](./images/log_in_link.png)

![Sign in Screen](./images/log_in_screen.png)

``Note: If you have forgotten, all information can be gathered in the stack under "Application Information".``

![Where to find username and password](./images/app_user_and_password.png)

### 6 Allow authentication

Click the green box that says "**Allow**."

![Authentication Screen](./images/allow_authentication.png)

You should now see the home page for Open On Demand (OOD).

![Open On Demand](./images/OOD.png)

## Lab Completed

Congratulations! You have successfully deployed the HPC Stack and Open Ondemand!

From this applciation you can deploy and run workloads on your HPC Lab as well as manage and view reports on the performance.

For further information on using OOD consult this resource:

``Resource``

This concludes this lab thank you for participating.

## Learn More

## Acknowledgements

* **Author:** Chris Wegenek
, Cloud Engineering 
* **Contributors:**
    - Germain Vargas, Cloud Engineering

* **Last Updated By/Date:** Chris Wegenek
, Cloud Engineering, December 2025