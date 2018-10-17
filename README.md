# keys
# ssh-keygen -t rsa -C 'myemail@mail.ru'

echo "# HomeJR" >> README.md
git init 
git add README.md
git commit -m "first commit" 
git remote add origin git@github.com:VraKorvis/HomeJR.git
git push -u origin master

git rm --cached 

ls -al ~/.ssh //check keys, to see if existing SSH keys are present:
Lists the files in your .ssh directory, if they exist



git log --pretty=format:"%h %ad | %s%d [%an]" --graph --date=short
    --pretty="..." — определяет формат вывода.
    %h — укороченный хэш коммита
    %d — дополнения коммита («головы» веток или теги)
    %ad — дата коммита
    %s — комментарий
    %an — имя автора
    --graph — отображает дерево коммитов в виде ASCII-графика
    --date=short — сохраняет формат даты коротким и симпатичным
~/.gitconfig (ctrl+h, ls -a)
[user]
	name = VraKorvis
	email = it.korvis@gmail.com
[core]
	autocrlf = false
	safecrlf = false
	editor = emacs
[alias]
  co = checkout
  ci = commit
  st = status
  br = branch
  hist = log --pretty=format:\"%h %ad | %s%d [%an]\" --graph --date=short
  type = cat-file -t
  dump = cat-file -p

~/.bash_aliases (for settings alias)
Проверьте наличие
if [ -f ~/.bash_aliases ]; then
. ~/.bash_aliases
fi
в вашем ~/.bashrc, и затем сделайте
 . ~/.bashrc (ввести в bash)
 alias gits='git status '
 alias ga='git add '
 alias gb='git branch '
 alias gc='git commit'
 alias gd='git diff'
 alias go='git checkout '
 alias gk='gitk --all&'
 alias gx='gitx --all'
 alias got='git '
 alias get='git '

