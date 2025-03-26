1. Creating an Env: 
```
conda create --prefix venv python=3.8 -y
```

2. bash terminal: 
```
conda create -p env python=3.8 -y source activate ./env
```

3. shortcut in bash terminal (Mac): 
```
conda create -p env python=3.8 -y && source activate ./env
```

4. Env activation: 
```
conda activate /Users/akshayy/dvc/env
```

5. To check what all packages are available:
```
pip3 list 
```

6. To install packages: 
```
pip3 install -r requirements.txt
```

7. Initializing git: 
```
git init 
```

8. Doesn’t want to push it in git repo: 
```
touch .gitignore
```

9. Steps to push your code to github repo:
```
Create a repo in github
```

```
git init
```

```
git add .
```

```
git commit -m "first commit"
```

```
git remote add origin https://github.com/akshayy1597/MLFlow1.git (copy the url from github)
```

```
git push -u origin main
```

10. CMD commands: 
```
mkdir dvc
```
cd dvc
```
code .
```

11. Whatever things will be written in the stage_1 and 2 will be locked in the dvc.lock file:
```
dvc repro
```

12. Will show you all the dependancies:
```
Dvc dag
```

13. pushing everything to github:
```
git add data.dvc && git commit -m "add data file"
```

14. To add the remote location and where we're using (/tmp/dvcstore) this folder as our central repo
```
mkdir tmp
```

```
cd tmp
```

15. to check the path of the folder 
```
pwd
```

```
mkdir dvcstore
```

```
dvc remote add -d myremote /tmp/dvcstore
```

16. pushing the changes:
```
dvc push
```

17. to retrive the changes:
```
dvc pull
```









