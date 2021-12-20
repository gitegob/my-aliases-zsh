# my-aliases-zsh
Aliases that make my development a breeze.

```bash
# add these to the ~/.zshrc (if you use zsh) or ~/.bashrc (if you use bash) file on linux or mac
# you can add or remove some to suit your own preferences

alias cl='clear'
alias c.='code .'
alias gst='git status'
alias ga='git add'
alias ga.='git add .'
alias gp='git push'
alias gpo='git pull origin'
alias gb='git branch'
alias gc='git commit'
alias gca='git commit --amend'
alias gpf='git push -f'
alias gd='git diff'
alias gco='git checkout'
alias gcob='git checkout -b'
alias glo="git log --graph --pretty=fuller"
alias gcan='git commit --amend --no-edit'
alias nr='npm run'
alias ni='npm i'
alias nid='npm i -D'
alias nr='npm run'
alias dev='yarn run start:dev'
alias yi='yarn install'
alias ya='yarn add'
alias yr='yarn run'
alias yad='yarn add -D'
alias sai='sudo apt-get install'
alias sau='sudo apt-get update'
alias fla='flutter pub add'
alias pyman='python manage.py'
alias pyserve='python manage.py runserver'
alias pyserve5000='python manage.py runserver 0.0.0.0:5000'
pinstall() {
	for var in "$@"
		do
    	pip install $var
		done
		pip freeze > requirements.txt
}
killport(){
	sudo kill -9 $(sudo lsof -t -i:$1)
 }
```
