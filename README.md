# summary-AWS-steps

## Step 1: Checking the App

First, I checked if the app was working properly:
- npm run build
- node ./dist/app.js
- 
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



## Step 6: i used sudo update (sudo apt update)
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/e701fa3a-13f0-40cb-8ba6-44a21a0bc595)

## Step 7: i used (sudo apt install awscli)

![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/9d3817cd-50f3-471d-9f54-c5ff786e391c)

## install node.js and curl: 
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/80cc3a1f-6b20-4eda-8c8f-e3d96e97e630)


## create infarasttructure folder and prepare-instance.sh file
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/c06a34fe-24f2-4546-a0a3-600a272efa36)

## create app.service file :
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/7dbd4be8-c8b0-4e31-bb11-9692d3516c95)


## making git clone by https:
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/e30b806c-a10a-471d-b834-2fa26e2c5661)

## cd to the app then instal npm 
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/b1bc0ad2-6b80-4701-b835-386da963490d)

## npm run build:
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/45628cea-15ae-47b5-8866-95e4fe4a4969)

## node ./dist/app.js
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/229a9340-9125-4e7f-8e52-0ddfc521649c)


## running the app using npm run dev :
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/ae19760e-d699-45fd-8acb-a692766ad4a4)

 ## make everything .json :
![image](https://github.com/salsabeel-alsahory/AWS-project/assets/100838183/4e40590c-2096-4c24-bcbe-e25db2ad00d4)

## create temblate luanche:
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/50cfba89-faa1-4499-bc66-309c5b243bfe)

## choose the correct sitting:
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/e9f8328b-218a-47ae-b9af-e524b651bd11)

we add this code to ouer temblete : 
```javascript
#!/bin/bash
set -e 

sudo apt update


curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -

sudo apt install nodejs  curl -y
git clone https://github.com/salsabeel-alsahory/AWS-project.git app
cd app 
npm install
npm run build
sudo mv ./infarastructure/app.service /etc/systemd/system/

sudo systemctl daemon-reload

sudo systemctl enable app.service
# sudo systemctl start app.service
sudo reboot 

```
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/a2da4efd-bca1-4f6e-addc-e62f43db3364)

## create auto scailing group :
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/0f72ad14-c748-4788-859d-c0c4a32a43a1)

## sitting of auto scsaling group : 

![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/d3daadef-1f0f-4b51-a7fe-322e1757e1cd)

## the group created successfuly :
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/6ef6913e-7d3f-4853-b598-c46227207747)

## go to Activity and check the instance:
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/a48cd2c0-eff9-491e-af73-26add4fae1c9)


## new instanc is created :
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/96a262eb-8205-4404-a109-3a7ae4004280)

## check the activity :
![image](https://github.com/salsabeel-alsahory/AWS-New-Project/assets/100838183/a79e5a58-35cf-4929-a917-7c04b6a46cce)


