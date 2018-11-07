# Call for Code Day Workshop

## Pre-requisite

IBM Cloud Account- [https://bit.ly/ibm-acct](https://bit.ly/ibm-acct)

## Steps

1. Clone the repo
2. Create an Action in IBM Cloud Functions
3. Import documents to Watson Discovery Service
4. Import Watson Assistant Workspace and update credentials
5. Try it out

## Architecture

![](readme-images/architecture-draft.png)

## Step 1: Clone the repo

`git clone https://github.com/IBMDevConnect/demo-callforcodeday.git`

## Step 2: Create an Action in IBM Cloud Functions

Step 2.1 Click the Hamburger to open the menu

  ![Hamburger](readme-images/1.png)

Step 2.2 Select **Functions** from menu

  ![Hamburger2](readme-images/2.png)

Step 2.3 Click **START CREATING** button

  ![Hamburger3](readme-images/3.png)

Step 2.4 Select **Create Action**

  ![Hamburger4](readme-images/4.png)

Step 2.5 Enter **Action Name**(copy Action Name in Notepad-required in later steps) and click **Create**

  ![Hamburger5](readme-images/5.png)

Step 2.6 Copy paste the code from [ibm_cloud_functions_code.txt](https://github.com/IBMDevConnect/demo-callforcodeday/blob/master/ibm_cloud_functions_code.txt) and click on Save

![Hamburger6](readme-images/6.png)

Step 2.7 Go back to Functions

  ![Hamburger7](readme-images/7.png)

Step 2.8 Click on **API Key**

  ![Hamburger8](readme-images/8.png)

Step 2.9 Take note of **Current Namespace** and **API Key** (required in later steps)

  ![Hamburger9](readme-images/9.png)

## Step 3: Import documents to Watson Discovery Service

Step 3.1 Navigate to Catalog > AI > Watson Discovery

![Hamburger9](readme-images/18.png)

Step 3.2 Create Watson Discovery Service

![Hamburger9](readme-images/19.png)

Step 3.3 Copy Service Credentials-Username & Password(required in later steps) and Launch Tool

![Hamburger9](readme-images/21.png)

Step 3.4 Click on **Upload your own data**

![Hamburger9](readme-images/22.png)

Step 3.5 Enter **Collection name** and **Create** the collection

![Hamburger9](readme-images/23.png)

Step 3.6 Upload the files that are there in the directory [discovery-data](https://github.com/IBMDevConnect/demo-callforcodeday/tree/master/discovery-data) by clicking on **Browse from computer**

![Hamburger9](readme-images/24.png)

Step 3.7 Copy the Collection ID & Environment ID (required in later steps)

![Hamburger9](readme-images/25.png)

## Step 4: Import Watson Assistant workspace

Step 4.1 Navigate to Catalog > AI > Watson Assistant

![Hamburger9](readme-images/10.png)

Step 4.2 Create Watson Assistant Service

![Hamburger9](readme-images/11.png)

Step 4.3 Launch Tool

![Hamburger9](readme-images/12.png)

Step 4.4 Import Workspace by clicking on Upload icon

![Hamburger9](readme-images/13.png)

Step 4.5 Choose JSON file [workspace-dc5ee9e6-a979-4cd4-a548-520252772a61.json](https://github.com/IBMDevConnect/demo-callforcodeday/blob/master/workspace-dc5ee9e6-a979-4cd4-a548-520252772a61.json) from the folder and click on Import

![Hamburger9](readme-images/14.png)

Step 4.6 Within Dialog Tab, click on **Anything Else** node

![Hamburger9](readme-images/15.png)

Step 4.7 Within JSON Editor, update **IBM Cloud Functions username, password, namespace and action name** (which was noted in Step 2.5 && Step 2.9 )

`NOTE: From the API Key-The segment before the colon (:) is your IBM Cloud Functions Username & segment after the colon is your IBM Cloud Functions Password`

![Hamburger9](readme-images/16.png)

Also, update **Discovery service username,password, environment id and collection id** (which was noted in Step 3.3 && Step 3.7)

![Hamburger9](readme-images/17.png)

## Step 5: Try it Out

Some questions you can try out are:

* Can the position of the moon or the planets affect seismicity?

* Can the ground open up during an earthquake?

![Hamburger9](readme-images/20.png)
