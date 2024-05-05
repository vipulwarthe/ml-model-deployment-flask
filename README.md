# ml-model-deployment-flask

Deploying ML models To the Web with Flask on AWS EC2 Instance

https://medium.com/shapeai/deploying-flask-application-with-ml-models-on-aws-ec2-instance-3b9a1cec5e13


-First we Create instance with ubuntu AMI with t2.medium instance type with 30GB storage 


   1   sudo apt-get update && sudo apt-get upgrade -y   (update the packages)   
   2   sudo apt install python3-venv -y          (install python environment)
   3   python3 -m venv mlpro                     (create environment name MLPRO)  
   4   source mlpro/bin/activate                 (activate the environment)
   5   deactivate                                (to deactivate the envirnoment)
   5   mkdir mlproject                           (create one project directory)
   6   cd mlproject                              (enter in project directory)

- you can directly clone the repo from github and start working...

-Login to your github account and create a new repo and paste cmds from github repo:

   7   echo "# Breast-Cancer-Prediction-Logistic-Regression-Project" >> README.md
   8   git add README.md
   9   git commit -m "First Commit"
   10  git status
   11  git branch -M main
   12  git branch
   13  git remote add origin https://github.com/vipulwarthe/Breast-Cancer-Prediction-Logistic-Regression-Project.git
   14  git push -u origin main

       git remote -v       (additional command)

-Create .gitignore file with python template in mlproject repo on github

   15  git pull    # It will pull the .gitignore file in VScode mlproject repo

-create setup.py and requirements.txt in mlproject repo add a code in setup.py & requirements.txt

-setup.py will be responsible in creating my ML application as a package
-setup.py is a module used to build and distribute Python packages
-requirements.txt file is a type of file that usually stores information about all the libraries, modules, and packages in itself that are used while developing a particular project

   16  pip install -r requirements.txt 
   17  git status
   18  git add .
   19  git status
   20  git commit -m "setup file added"
   21  git push -u origin main
  
IMP :  if any error occured while run "git push -u origin main" command then use below command to resolve the issue:
       git pull --rebase origin main
