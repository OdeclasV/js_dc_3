--------- Insert Notes ---------

### Useful commands from "Git assignment":   
-git log --summary (summary of commits and changes)  
-git -u origin master (-u tells git to continue using "origin and master")  
-git diff HEAD (*diff* shows changes from last commit, *HEAD* selects most recent commit)  




### Useful commands from "Terminal customization":   
parse_git_branch() {
  git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}  

export PS1="\W $(parse_git_branch)"


--------- FIN ---------