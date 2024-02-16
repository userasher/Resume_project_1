# Resume_project_1
Deploying my 1st Nodejs app on a remote AWS instance as an IAM user

How to login into remote VM instance with linux terminal?
=>Create a VM using oracle virtual box and login using a password into your VM.
=>Press ctrl+alt+t in you VM. It is a keyboard shortcut to open terminal in your ubuntu machine.
=>Type following commands to prepare your VM for this project.
  =dfkjgdfjghdfg

Prerequisites:
You will need an AWS account. Amazon provides a free tier account in which almost all the services are provided to the user on the trial basis.

Step1: Create a FREE tier AWS account and login to a management console.

Step2: Just search EC2 in the search bar and click on it. 
After that you can see a ORANGE launch instance button, click launch instance.
You will be redirected to a LAUNCH AN INSTANCE page
  1)write you EC2 instance name
  2)select an application and OS image (select ubuntu)
  3)Make sure that next option of selecting AMAZON MACHINE IMAGE has free tier elegible written on it(or eles you will have to pay for it)
  4)same goes for instance type(everything bydefault is selected to be free tier eligible)
  5)Then comes the KEY PAIR. click on CREATE NEW KEY PAIR => a file with .pem extension will be downloaded to your local machine automatically.
  6)Rest all let it be as it is for now scroll down till the end of the page.
  7) CLCIK ON LAUNCH INSTANCE BUTTON at the bottom of the page.

Since we deploying this app as an IAM user you need to use the IDENTITY AND ACCESS MANAGEMENT(IAM) SERVICE provided by AWS.

Step3: Click on the aws logo at the left upper corner of the screen which will take you to the management console.
  =>Search for IAM in search bar and click on it, you will be redirected to IAM dashboard.
  
  =>Now these are some important steps follow them carefully
  
    ==>In the left hand side panel under access managament there is an option called users, click on it.
    ==>You will be redirected to create user page.
    ==>Click create user button and give a name to an IAM user account.
    ==>There will be a 2 options:  select ====>I WANT TO CREATE AN IAM user option and set a custom password and uncheck ====> Users must create a new password at next sign-in - Recommended option
    ==>Then you will need to set permissions for the user, select ATTACH POLICIES DIRECTLY options on your screen.
    ==>There are many policies but for now select ADMINISTRATORACCESS policy in the list mentioned and click next.
    ==>You will be redirected to review and create page, at the bottom of this page click CREATE USER button.
    ==>After this an IAM USER will be created with host account as your AWS Account and a credential file will be downloaded to your local machine which consists of the:
        ==>username and password you have set for your IAM user account.
        ==>the root account id.
        ==>some other details.
    ==>Now go back to IAM user signin page and login using your root accountid, account name and password which you can find in file you downloaded in the above step.

That's it now you are ready to deploy your first app.

Now after logging in as an IAM user you will see a similar page as that of AWS management console

Steps to be followed from now on:
STEP1: Create an EC2 instance.(refer the start of thIS README)
STEP2: Now login in into your remote EC2 instance you just created using AWS.(REFER TO START OF THIS README)
STEP3: important steps from now follow accordingly
      ==>















  
  


    
