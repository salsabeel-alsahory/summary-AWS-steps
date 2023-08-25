# summary-AWS-steps

## Step 1: Checking the App

**Description**: I started by building the app and running it to ensure it's functioning as expected. This helps in identifying any initial issues.

## Step 2: Creating a Book Instance

**Description**: I created a new instance to deploy the app on AWS. This instance will host the application and allow users to access it.
**Link**: ![Creating a Book Instance](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/d430e22d-e82d-4301-be3e-a2e7d501c4ab)

## Step 3: Connecting to the Instance

**Description**: After setting up the instance, I navigated to the instance details and accessed the "Connect" section to retrieve SSH connection information.
**Link**: ![Connecting to the Instance](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/cc21beec-6edf-4c44-bc79-a63a8aa6a990.png)

## Step 4: Copying SSH and Pasting in the Terminal

**Description**: I copied the SSH command provided in the AWS console and pasted it into my local terminal. This connects my local machine to the AWS instance.
**Link**: ![Copying SSH](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/f38cd329-8b6d-4820-a6b0-d71981bd9246)

## Step 5: Connect the SSH on My Device

**Description**: I used the SSH command along with the private key ("booksKeyPair.pem") to establish a secure connection to the AWS instance from my local machine.
**Link**: ![Connecting SSH](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/4f1a8b9c-2942-4197-8159-71fe6b4b3e22)

## Step 6: Updating the System

**Description**: I ran the command `sudo apt update` to update the package lists for upgrades and installations on the AWS instance.
**Link**: ![Updating System](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/e701fa3a-13f0-40cb-8ba6-44a21a0bc595)

## Step 7: Installing AWS CLI

**Description**: I used the command `sudo apt install awscli` to install the AWS Command Line Interface, which allows interaction with AWS services from the terminal.
**Link**: ![Installing AWS CLI](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/9d3817cd-50f3-471d-9f54-c5ff786e391c)

## Install Node.js and Curl

**Description**: I installed Node.js and Curl on the AWS instance, which are required to run and manage the application.
**Link**: ![Installing Node.js and Curl](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/80cc3a1f-6b20-4eda-8c8f-e3d96e97e630)

## Creating Infrastructure Folder and prepare-instance.sh File

**Description**: I created an "infrastructure" folder and prepared a shell script named "prepare-instance.sh" to automate the setup process.
**Link**: ![Creating Infrastructure Folder](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/c06a34fe-24f2-4546-a0a3-600a272efa36)

## Creating app.service File

**Description**: I created an "app.service" file that defines the service configuration for running the app using systemd.
**Link**: ![Creating app.service File](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/7dbd4be8-c8b0-4e31-bb11-9692d3516c95)

## Cloning the Repository via HTTPS

**Description**: I cloned the app repository from GitHub using the HTTPS link. This will bring the app's code to the AWS instance.
**Link**: ![Cloning the Repository](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/e30b806c-a10a-471d-b834-2fa26e2c5661)

## Installing Dependencies and Building the App

**Description**: I navigated to the app directory and used `npm install` and `npm run build` to install dependencies and build the app.
**Link**: ![Installing Dependencies and Building](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/b1bc0ad2-6b80-4701-b835-386da963490d)

## Running the App

**Description**: I ran the app using `npm run dev` to test its functionality.
**Link**: ![Running the App](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/ae19760e-d699-45fd-8acb-a692766ad4a4)

## Creating Template Launch Configuration

**Description**: I created a launch configuration template that includes the necessary setup steps for the instance.
**Link**: ![Creating Template Launch](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/50cfba89-faa1-4499-bc66-309c5b243bfe)

## Configuring Auto Scaling Group

**Description**: I configured an auto scaling group based on the launch configuration to ensure the availability and reliability of the application.
**Link**: ![Configuring Auto Scaling](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/d3daadef-1f0f-4b51-a7fe-322e1757e1cd)

## Checking Instance Activity

**Description**: I monitored the instance activity to ensure that new instances were being launched and scaled as needed.
**Link**: ![Checking Instance Activity](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/a48cd2c0-eff9-491e-af73-26add4fae1c9)
