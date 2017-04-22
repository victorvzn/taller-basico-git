# Learning git

Working directory <> Staging Area[INDEX] <> Repository	

git init
git status
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
	git log --oneline
	git log --oneline --decorate
	git log --oneline --decorate --graph
	git log --oneline --decorate --all --graph
git diff
	git diff <hash7> <hash7>
	git diff HEAD~1 HEAD
git branch
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