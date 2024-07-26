# ml-model-deployment-flask

Deploying ML models To the Web with Flask on AWS EC2 Instance

https://medium.com/shapeai/deploying-flask-application-with-ml-models-on-aws-ec2-instance-3b9a1cec5e13


## First we Create instance with ubuntu AMI with t2.micro instance type with 30GB storage 


    sudo apt-get update && sudo apt-get upgrade -y       (update the packages)   

    sudo apt install python3-venv -y                     (install python environment)

    python3 -m venv mlpro                                (create environment name MLPRO)  

    source mlpro/bin/activate                            (activate the environment)

    deactivate                                           (to deactivate the envirnoment)

    mkdir mlproject                                      (create one project directory)

    cd mlproject                                         (enter in project directory)

## you can either directly clone the repo or create new repo in github and start working. so we are going to create new repo, please follow below steps:

## Login to your github account and create a new repo and paste cmds from github repo:

    echo "# Breast-Cancer-Prediction-Logistic-Regression-Project" >> README.md
   
    git add README.md
   
    git commit -m "First Commit"
   
    git status
   
    git branch -M main
   
    git branch
   
    git remote add origin https://github.com/vipulwarthe/ml-model-deployment-flask.git
   
    git push -u origin main

    git remote -v       (additional command)

## Create .gitignore file with python template in mlproject repo on github

    git pull    # It will pull the .gitignore file in VScode mlproject repo

## create setup.py and requirements.txt in mlproject repo add a code in setup.py & requirements.txt

* setup.py will be responsible in creating my ML application as a package
* setup.py is a module used to build and distribute Python packages
* requirements.txt file is a type of file that usually stores information about all the libraries, modules, and packages in itself that are used while developing a particular project

      pip install -r requirements.txt 
   
      git status
   
      git add .
   
      git status
   
      git commit -m "setup file added"
   
      git push -u origin main
  
## IMP :  if any error occured while run "git push -u origin main" command then use below command to resolve the issue:

    git pull --rebase origin main

## Deploy application:

    python3 app.py
