## Aliases

Add

```
if [ -f ~/.bash_aliases ]; then
. ~/.bash_aliases
fi
```

into `.bashrc` and perform `source ~/.bashrc` after each edit of `.bash_aliases`

#### Useful aliases

```
alias dc='docker-compose'
```


#### Git aliases
```
git config --global alias.co checkout  
git config --global alias.br branch  
git config --global alias.cm commit  
git config --global alias.st status  
  
git config --global alias.ll "log --oneline --decorate" 
git config --global alias.pos "pull origin staging"  
git config --global alias.amend "commit --amend"  
git config --global alias.append "commit --amend --no-edit"  
git config --global alias.hist "log --pretty=format:'%h %ad | %s%d [%an]' --graph --date=short"  
git config --global alias.last 'log -1 HEAD'  
git config --global alias.who "shortlog -n -s --no-merges"  
```  
Add to `.gitconfig`  
```
ri = "!ri() { git rebase -i HEAD~$1; }; ri"  
la = "!git config -l | grep alias | cut -c 7-"  
```
