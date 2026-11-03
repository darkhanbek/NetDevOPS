настройка метаданных
git config --global user.name Darkhan
git config --global user.email darkhanbek@gmail.com



имя основной ветки по умолчанию(main вместо master)
git config --global init.defaultBranch main


создаем первый репозиторий
mkdir ~/git-lab
cd ~/git-lab


инициализция репозитория
git init


создаем первый файл
echo "my first commit" > hello.txt


посмотреть статус
git status


добавляем файл в staging для подготовки к commit
git add hello.txt


делаем commit
git commit -m "first commit: add hello.txt"


проверка истории
git log


добавляем второй запись
echo "add second column" >> hello.txt


смотрим что изменилось
git diff


теперь комиттим изменения
в итоге у нас получится два коммита и к любому из них можно будет откатится
git add hello.txt
git commit -m "add second column in hello.txt"
git log
