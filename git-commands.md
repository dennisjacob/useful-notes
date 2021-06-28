git init

git config --list

git config --global --list

git add <file_name>
git add .
git add *.txt

git commit -m "Comment"  -m "Description"

git remote add      origin git@github.com:dennisjacob/demo.git
git remote set-url  origin git@github.com:dennisjacob/demo.git
git remote -v


#Create a new branch
git  checkout -b your_local_branch
git push -u origin your_local_branch   # to create the branch at remote
