# AWS Project

## Step 1: Checking the App

First, I checked if the app was working properly:
- npm run build
- node ./dist/app.js

![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/555f6bc7-adc8-409c-9467-04d89d14d29a)
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/3269aa0c-fa0b-403e-a76f-8ac9d98a214d)


## Step 2: Creating a Book Instance

Next, I created a new Book instance:

![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/d430e22d-e82d-4301-be3e-a2e7d501c4ab)


## Step 3: Connecting to the Instance

After creating the instance, I selected the instance we were working on and went to the connect section:

![Connect Instance](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/cc21beec-6edf-4c44-bc79-a63a8aa6a990.png)


## Step 4: Copying SSH and Pasting in the Terminal

Then, I copied the SSH command provided and pasted it into the terminal:
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/f38cd329-8b6d-4820-a6b0-d71981bd9246)


## Step 5: Connect the SSH on My Device Using This Command (ssh -i "booksKeyPair.pem" ubuntu@ec2-52-90-81-143.compute-1.amazonaws.com)

![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/4f1a8b9c-2942-4197-8159-71fe6b4b3e22)


## Step 6: Updating the System

I used the command `sudo apt update` to update the package lists for upgrades and installations on the AWS instance.
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/e701fa3a-13f0-40cb-8ba6-44a21a0bc595)


## Step 7: Installing AWS CLI

I used `sudo apt install awscli` to install the AWS Command Line Interface on the instance.
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/9d3817cd-50f3-471d-9f54-c5ff786e391c)


## Install Node.js and Curl

I installed Node.js and Curl on the AWS instance, required to run and manage the application.
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/80cc3a1f-6b20-4eda-8c8f-e3d96e97e630)


## Creating Infrastructure Folder and prepare-instance.sh File

I created an "infrastructure" folder and prepared a shell script named "prepare-instance.sh" to automate the setup process.
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/c06a34fe-24f2-4546-a0a3-600a272efa36)


## Creating app.service File

I created an "app.service" file that defines the service configuration for running the app using systemd.
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/7dbd4be8-c8b0-4e31-bb11-9692d3516c95)


## Making Git Clone by HTTPS

I cloned the app repository from GitHub using the HTTPS link.
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/e30b806c-a10a-471d-b834-2fa26e2c5661)


## Installing Dependencies and Building the App

I navigated to the app directory, used `npm install`, and `npm run build` to install dependencies and build the app.
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/b1bc0ad2-6b80-4701-b835-386da963490d)


## Running the App

I ran the app using `npm run dev` to test its functionality.
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/ae19760e-d699-45fd-8acb-a692766ad4a4)


## Making Everything .json

I made every aspect of the app configuration .json-based.
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/4e40590c-2096-4c24-bcbe-e25db2ad00d4)


## Creating Template Launch Configuration

I created a launch configuration template that includes the necessary setup steps for the instance.
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/50cfba89-faa1-4499-bc66-309c5b243bfe)


## Configuring Auto Scaling Group

I configured an auto scaling group based on the launch configuration for high availability and reliability.
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/d3daadef-1f0f-4b51-a7fe-322e1757e1cd)


## Checking Instance Activity

I monitored the instance activity to ensure that new instances were being launched and scaled as needed.
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/a48cd2c0-eff9-491e-af73-26add4fae1c9)


## New Instance is Created

A new instance was successfully created.
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/96a262eb-8205-4404-a109-3a7ae4004280)


## Checking the Activity

I continued to check the instance activity for any updates.
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/a79e5a58-35cf-4929-a917-7c04b6a46cce)
