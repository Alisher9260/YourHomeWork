# Руководство по работе с системой контроля версий Git
Команды Git:

##Базовые##

* *git init* - команда,инициализирующая репозиторий в текущей директории;
* *git clone* -  команда для создания локального клона (рабочей копии)
* *git status* - команда , отображающая статус текущего документа;
* *git push* - команда, привязывающая локальный репозиторий с основным
* *git log* - команда, которая демонстрирует последние 2 сохраненных версии документа с возможностью просмотра всех предидущих версий. При добавлении строки -- graph - на экран терминала выводится дерево всех коммитов для всех веток
* *git add* - команда, которая добавляет изменения для последующего сохранения в документе. 
* *git commit* - команда , которая позволяет дополнить комментарием и зафиксировать выполненные в документе изменения
* *git checkout master* - команда, позволяющая вернуться на основную ветку работы с документом
* *git branch* - команда, позволяющая просмотреть все существующие ветки
* *git merge _branch name_* - команда, позволяющая совместить ветку с веткой "мастер"
* *git diff* - команда, позволяющая просмотреть разницу между ветками 
* gitignore - cпециальный тип файлов, шаблон которых сопоставляясь с исходным файлом игнориуется Git.
** работа с удаленными репозиториями **
При работе с репозиториями в GitHub возможны следующие процессы:
--создание нового репозитория на коммандной строке с последующим выполнением комманд:
    git init
    git add
    git commit -m "начальный комит"
    git branch -M main (базовая ветка)
    git remote add origin (*команда,позволябщая отправить созданный репозиторий из компьютера в GIThub*) __cсылка на репозиторий__
    git push -U (*upstream*) origin main
--внедрение (push) существующего репозитория из коммандной строки

Также при работе возможно создание локальных побочных веток с локального репозитория с помощью их создания командой git branch  
Для отправки информации из локальной ветки в удаленный репозиторий используется команда git push --set - upstream origin __название ветки__
для того чтобы забрать изменения из удаленного репозитория в локальный используется команда git pull