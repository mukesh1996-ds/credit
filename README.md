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
Stage 1:
command to create the get_data.py file
```bash
cd .> get_data.py
```
create a python file name get_data.py and this file will help you to get your data.
command to execute get_data.py file is:  
```bash
python src\get_data.py
```
By this your first stage is completed.

Stage 2:
we will create a file called load_data.py which will run the data and store it in data\raw folder
```bash
cd .> load_data.py
python src\load_data.py
```
also open dvc.yaml file and enter all the stages init and to check all the stages 
command it 
```bash
dvc repro
```


