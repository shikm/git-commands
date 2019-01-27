# Commands

___

### GIT Version:

<pre>
git --version
</pre>

### Set name credential:

<pre>
git config --global user.name <b>"maxim.shik"</b>
</pre>

### Set E-mail credential:

<pre>
git config —-global user.email <b>"maxim.shikzzy@gmail.com"</b>
</pre>

### See all configurations: 

<pre>
git config —-list
</pre>

### See own custom configurations: 

<pre>
git config --list --global
</pre>

### Help Command 

```
git help  
```

### Get help from a specific command 

<pre>
git help <b>commit</b>
</pre>

### Create a Repository 

<pre>
git init
</pre>

### Delete a Repository

<pre>
rm -rf .git
</pre>

### Add a file 

<pre>
git add <b>index.html</b>
</pre>

### Add multiple files 
<pre>
git add <b>index.html index.js</b>
</pre>

### Add all files 

<pre>
git add .
</pre>

### Add all the files in the current directory by their extension: 

<pre>
git add <b>*.js</b>
</pre>

### Add all the files that are in a folder: 

<pre>
git add <b>css/</b>
</pre>

### Add all the files by their extension that are inside a folder: 

<pre>
git add <b>src/*.js</b>
</pre>

### See modified files 

<pre>
git status
</pre>

### See the modified files without so much information: 

<pre>
git status -s
</pre>

### See the modified files and in which branch we are working:

<pre>
git status -sb
</pre>

### Delete a file that was in the staging area:  

<pre>
git reset <b>index.js</b>
</pre>

### Delete a file that was in the staging area by their extension:

<pre>
git reset <b>*.js</b>
</pre>

### Commit Changes:

<pre>
git commit -m <b>'initial commit'</b>
</pre>

### See all the commits that we did:

<pre>
git log
</pre>

### See all the commits that we did in a pretty way:

<pre>
git log --oneline --decorate --all --graph
</pre>

___

### See all the changes that happened between the working file and the staging file:

<pre>
git diff
</pre>

### See all the changes that happened between the staging area file and the commited file:

<pre>
git diff --staged
</pre>

### Recover Files:

<pre>
git checkout .
</pre>

### Discard changes in working directory:

<pre>
git checkout -- <b>README.md</b>
</pre>

### Edit last commit message:

<pre>
git commit --amend -m <b>'Update this message'</b>
</pre>

### Add or Back to the last commit:

<pre>
git reset --soft HEAD^
</pre>

### Return to a specific commit in a weak way:

<pre>
git reset --soft <b>f6d5669a7a941075b42b9336a2dd427d34bc00b9</b>
</pre>

### Return to a specific commit in a hard way:

<pre>
git reset --hard <b>f6d5669a7a941075b42b9336a2dd427d34bc00b9</b>
</pre>

### List of originated commits:

<pre>
git reflog
</pre>

### Rename Files:

<pre>
git mv <b>index.js app.js</b>
</pre>

### Delete Files:

<pre>
git rm <b>app.js</b>
</pre>

## Branches

### Create a branch:

<pre>
git branch <b>first-step</b>
</pre>

### List all of the branches in your repository:

<pre>
git branch
</pre>

### Switch between branches:

<pre>
git checkout <b>first-step</b>
</pre>

### Create and move to a branch in a single command:

<pre>
git checkout -b <b>first-step</b>
</pre>

## Merge branches:

### Go back to the master branch:

<pre>
git checkout master
</pre>

### Now run the next command:

<pre>
git merge <b>first-step</b>
</pre>

### Once merged we can proceed to delete the branch:

<pre>
git branch -d <b>first-step</b>
</pre>

## Tags

### Create a tag:

<pre>
git tag -a <b>v1.0.0</b> -m <b>"Version 1.0.0"</b>
</pre>

### Insert a tag in a specific commit:

<pre>
git tag -a <b>v0.1.0 f6d5669a7a941075b42b9336a2dd427d34bc00b9</b> -m <b>'Alpha Version'</b>
</pre>

### See all Tags:

<pre>
git tag
</pre>

### See the tag message:

<pre>
git show <b>v1.0.0</b>
</pre>

### Delete a tag:

<pre>
git tag -d <b>v0.1.0</b>
</pre>

## Stash

### Creation:

<pre>
git stash
</pre>

### Get the list:

<pre>
git stash list
</pre>


# Github

### Once we create a repository, we can add it to the remote server:

<pre>
git remote add origin <b>repositoryName.git</b>
</pre>

### See the remote sources of our repository:

<pre>
git remove -v
</pre>

### Push:

<pre>
git push -u origin master
</pre>

### Push the tags:

<pre>
git push --tags
</pre>

### Ignore Files:

<pre><b>You can also create a global .gitignore file, which is a list of rules for ignoring files in every Git repository on your computer.</b></pre>

<pre>
.DS_Store
.idea
node_modules
package-lock.json
</pre>

### Pull:

<pre>
git pull
</pre>

### Clone a Repository:

<pre>
git clone <b>repositoryName.git</b>
</pre>

### Clone a repository in a specific folder:

<pre>
git clone <b>repositoryName.git my-folder</b>
</pre>

___

