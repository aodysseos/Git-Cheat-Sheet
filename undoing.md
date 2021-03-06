# :man_facepalming: Undoing

:point_left:[BACK](README.md)

### 1. Undo `git add` before commit

Git Commnad 	        		  			| Description
----------------------------------------- 	| ---------------
**`git reset <file>`** 			  			| unstage specific file
**`git reset`** 			  				| unstage all files

### 2. Return to previous commit

Git Commnad 	        		  			| Description
----------------------------------------- 	| ---------------
**`git reset HEAD~ --soft`** 			  	| undo the last commit, but leave the changes available
**`git stash`**  						  	| stash changes
**`git checkout correct-branch`**  	  		| move to the correct branch
**`git stash pop`**  					  	| apply stash
**`git add . # or add individual files`**  	| add changes to correct branch
**`git commit -m "your message here"`**  	| now your changes are on the correct branch 

### 3. Amend the message of my last commit

Git Commnad 	        		  		    | Description
------------------------------------------- | ---------------
**`git commit --ament`** 			  		| follow prompts to change the commit message, save and exit using `:x`

### 4. Accidentally committed to the wrong branch

Git Commnad 	        		  		    | Description
------------------------------------------- | ---------------
**`git reset HEAD~ --soft`** 			  	| undo the last commit, but leave the changes available
**`git stash`** 						  	| stash changes
**`git checkout correct-branch`** 	  	    | move to the correct branch
**`git stash pop`** 					  	| apply stash
**`git add . # or add individual files`**   | add changes to correct branch
**`git commit -m "your message here"`** 	| now your changes are on the correct branch

### 5. Accidentally committed to the wrong branch (Cherry-Pick)

Git Commnad 	                        	| Description
------------------------------------------- | ---------------
**`git checkout correct-branch`**        	| move to the correct branch
**`git cherry-pick master`**		        | grab the last commit to master
**`git checkout master`**	  				| move to master
**`git reset HEAD~ --hard`**				| delete it from master

### 6. Remove file or directory after adding it in to `.gitignore` file

Git Commnad 	                        	| Description
------------------------------------------- | ---------------
**`git rm -r --cached <file-name>`** OR **`<directory>/*'`** | the staged content has to match the tip of the branch allowing the file to be removed from the index
**`git commit -m "<your message>"`**    					 | commit your changes
**`git push <remote> <branch>`**        					 | push your changes 

:point_left:[BACK](README.md)

