# Learning git

Working directory <> Staging Area[INDEX] <> Repository	

```bash 
git init
git status
git add
	git add .
	git add <file> 
	git checkout -- <file>   [ to discard changes in WD ]
	git diff
	git reset HEAD <file>    [ to unstage ]
git commit -m "message"
	git commit --amend       [ to add more commir to the last one ]
	git reset <hash7>        [ to untage commit]
	git reset --hard <hash7> [  ]
	git reset --soft <hash7> [  ]
	git checkout -- <file>   [ to discard changes in WD ]
	git revert HEAD
	git revert --no-commit HEAD
		git revert --continue
git log
	git log
	git log --oneline
	git log --oneline --decorate
	git log --oneline --decorate --graph
	git log --oneline --decorate --all --graph
git diff
	git diff <hash7> <hash7>
	git diff HEAD~1 HEAD
git branch
	git branch
	git branch --all
	git branch <branch_name>
	git checkout <branch_name> [ to switch branch ]
	git checkout -b <branch_name> [ creamos y cambiamos a un nuevo branch]
	git branch -m <before_name> <new_name> [ rename branch ]
	git branch -d <branch_name>   [ delete a branch ]
git merge
	git merge <branch_name> [fast-forward, recursive]
	git merge --abort
git config
	git config --global --get-regexp alias [ List all alias ]
	git config --global --unset alias.lodag [ Delete alias ]
	git config --global alias.lodag 'log --oneline --decorate --all --graph | cat'
	git config --global alias.co checkout
	git config --global alias.br branch
	git config --global alias.ci commit
	git config --global alias.st status
	git config --global alias.unstage 'reset HEAD --'
	git config --global alias.last 'log -1 HEAD'
git tag
	git tag v0.1.0 [ Crea un tag del HEAD]
	git tag v0.2.0 <hash7> [ Crea un tag en un commit especifico ]
	git checkout <tag_name> [ Cambiamos a un tag ]
	git tag -l [ tag list ]
	git tag -d v.0.1.0 [ Borrar un tag ]
git stash
	git stash
	git stash list
	git stash apply
	git stash drop
	git stash save "<message>"
git remote
	git remote add origin <url_repository>
	git remote -v [  ]
git clone
	git clone <url_repository>
git push
	git push <remote_name> <remote_branch>
		git push origin master
git pull
	git pull <remote_name> <remote_branch>
	git pull origin master
git fetch [ preguntar a un remoto si hay cambios y descargarlas solamente ]
	git fetch <remote_name>
	git fetch origin
```

