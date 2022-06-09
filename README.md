# Removing sensitive text steps

1) Create a replacements.txt file with the text you want to replace followed by "==>" and the new text 
* e.g myPassword123==>This will replace the text on the left
2) Run the command to replace the text in the whole repository
* git filter-repo --replace-text replacements.txt --force
3) Add back the remote that has been automatically removed for security reasons 
* git remote add origin https://github.com/GeorgeDoitsinis/History_Emulator.git
4) Push the origin main with -u tag to connect our main local branch with the remote
* git push -u origin main --force

