# keys
# ssh-keygen -t rsa -C 'myemail@mail.ru'

# FirstRepo
# echo "# HomeJR" >> README.md
# git init 
# git add README.md
# git commit -m "first commit" 
# git remote add origin git@github.com:VraKorvis/HomeJR.git
# git push -u origin master

# ls -al ~/.ssh //check keys, to see if existing SSH keys are present:
# Lists the files in your .ssh directory, if they exist

# формат вывода
# git log --pretty=format:"%h %ad | %s%d [%an]" --graph --date=short
    --pretty="..." — определяет формат вывода.
    %h — укороченный хэш коммита
    %d — дополнения коммита («головы» веток или теги)
    %ad — дата коммита
    %s — комментарий
    %an — имя автора
    --graph — отображает дерево коммитов в виде ASCII-графика
    --date=short — сохраняет формат даты коротким и симпатичным

