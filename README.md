# Fraud transaction detection

Create a new environmnet and activate the environmnet 
```bash
conda create -n credit python=3.7 -y
conda activate credit
```
Create a new file name requirements.txt
```bash
cd .> requirements.txt
pip install -r requirements.txt
```
Then create a new file name template.py
```bash
cd .> template.py
```
This file will create a basic structure for my project as similar to cookicutter.
To run the python file 
```bash
python template.py
```
Initilize git and dvc command
```bash
git init
dvc init
```
Add tracking dataset to the dvc
```bash
dvc add data_given/credit.csv
```
This will create a .dvc file and that file will be pushed to the rep.
commit your project to git
```bash
git remote add origin https://github.com/mukesh1996-ds/credit.git
git branch -M main
git push origin main
```
Stages to create a project
1. create a python file name get_data.py and this file will help you to get your data.
command to execute get_data.py file is:  
```bash
python src\get_data.py
```
By this your first stage is completed.




