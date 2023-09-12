# my-aliases-zsh
Aliases that make my development a breeze.

It is better to have [Oh-my-zsh](https://github.com/ohmyzsh/ohmyzsh) installed since it provides some basic aliases out of the box as well.

```bash
# add these to the ~/.zshrc (if you use zsh) or ~/.bashrc (if you use bash) file on linux or mac
# you can add or remove some to suit your own preferences

alias cl='clear'
alias c.='code .'
alias ga.='git add .'
gpo(){
        git switch $1 && git pull origin $1
}
alias gpf='git push -f'
alias glo="git log --pretty=format:'# %ad %H %s' --date=short --first-parent --reverse"
alias gcan='git commit --amend --no-edit'
alias gs='git switch'
alias gsc='git switch -c'
alias nr='npm run'
alias ni='npm i'
alias nid='npm i -D'
alias nr='npm run'
alias dev='yarn run start:dev'
alias yi='yarn install'
alias ya='yarn add'
alias yr='yarn run'
alias yad='yarn add -D'
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
