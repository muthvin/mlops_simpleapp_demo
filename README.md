Reference: https://github.com/c17hawke/simple-dvc-demo

1. Create env
```bash
conda create -n wineq python=37 -y 

2. activate env
```bash
conda activate

3. create a requirment file
install the req
```bash
pip install -r requirements.txt

4. Create template.py file
    using template, create folder structure,yaml files and other files
5. Create a folder <data_given>
    Transfer the data to the folder
    link: :https://drive.google.com/drive/folders/18zqQiCJVgF7uzXgfbIJ-04zgz1ItNfF5
6. git init
   dvc init
   dvc add data_given/winequality.csv
   # above step to have the original version of the data in dvc format
   git add .
   git commit -m "first commit" 
   # create git repostory in github:and follow 3 commands
   git remote add origin https://github.com/muthvin/mlops_simpleapp_demo.git
   git branch -M main
   git push -u origin main
7. Start updating params. yaml
   Upload the created params.yaml to github
8. create src/get_data.py 
    - includes reading the csv as pandas df
    - return df as output
9. create src/load_data.py
    - modify the col_name
10. create dvc.yaml
11. Execute dvc repro
    