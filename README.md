## Git Complete: The definitive, step-by-step guide to Git 
![GIT](gitcomplete.jpg)

Boosting my Git skils.

## Progress/Curriculum

- [x] 01 - Introduction 
- [x] 02 - Git Installation
- [x] 03 - Git Quick Start
- [x] 04 - Text Editor Installation
- [ ] 05 - 
- [ ] 06 - 
- [ ] 07 - 
- [ ] 08 - 
- [ ] 09 - 
- [ ] 10 -
- [ ] 11 - 
- [ ] 12 - 
- [ ] 13 - 


## Notes/Commands


Set name
- git config --global user.name "Your Name"
Set email
- git config --global user.email "yourEmail@here.com"
List name and email
- git config --global --list
Clone my repository to local system
- git clone https://github.com/developersCradle/starter-web 

-- Staging area building several changes before committed as 1 unit

Pushing(origin refers to the GitHub copy of our repository, master is branch name on GitHub)
- git push origin master

List all the configuration from global or from user level
- git config --global --list

Adding core ediotor to git config
git config --global core.editor "notepad++.exe -multiInst -nosession"

`.bash_profile` to home directory
Configure Notepad++ with git

Testing default editor is working, editing git config file
git config --global -e

Ask git status
- git status

- [hipsum](https://hipsum.co/)
- `origin/master` origin is reference to github repository, and master is branch
- git status command keeps track of origin master
- best practise is do pull before push

- Basic Git Workflow
<img src="BasicGitWorkflow.PNG" alt="alt text" width="300"/>

- Git Tracked file
<img src="gitTracking.PNG" alt="alt text" width="300"/>

Listing tracked files
- git ls-files

Git status only shows first level of directories

Adding file recursively
- git add .

Backingout chenages form staging area
- git reset HEAD "filename.here"

Going back state when files were last committed
- git checkout -- "filename.here"

When moving or renaming files in encouraged to to use git mv
- git mv
Moving file one level down
mv level2.txt ..

