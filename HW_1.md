# Terminal
<img loading="lazy" src="https://hasura.io/blog/content/images/downloaded_images/setting-up-git-bash-for-windows-e26b59e44257/1-Je4yF-xdHEluVvmS0qw8JQ.png">

## HW_1

1. Посмотреть где я - **pwd**
2. Создать папку - **mkdir 33dir**
3. Зайти в папку - **cd 33dir**
4. Создать 3 папки - **mkdir f1 f2 f3**
5. Зайти в любую папку - **cd f1**
6. Создать 5 файлов (3 txt, 2 json) - **touch 1.txt 2.txt 3.txt 4.json 5.json**
7. Создать 3 папки - **mkdir f11 f12 f13**
8. Вывести список содержимого папки - **ls -la**
9. Открыть любой txt файл - **vim 1.txt**
10. Написать туда что-нибудь, любой текст - **Клавиша i, затем ввод текста:
                                                                     Hello, World! 
                                                                     Never give up!**
11. Сохранить и выйти - **ESC+Shift : wq**
12. Выйти из папки на уровень выше - **cd ..**
13. Переместить любые 2 файла, которые вы создали, в любую другую папку - **mv {f1/1.txt,f1/2.txt} f2**
14. Скопировать любые 2 файла, которые вы создали, в любую другую папку - **cp 8.txt 9.txt  f3**
15. Найти файл по имени - **find . -name “1.txt”**
16. Просмотреть содержимое в реальном времени - **tail -f 1.txt**, **закончить команду ctrl+C**
17. Вывести несколько первых строк из текстового файла - **head -5 1.txt**
18. Вывести несколько последних строк из текстового файла - **tail -2 1.txt**
19. Просмотреть содержимое длинного файла - **less 1.txt**
20. Вывести дату и время - **date**  

=========

**Задание***
1. Отправить http запрос на сервер.  
http://162.55.220.72:5005/terminal-hw-request  
**Curl  http://162.55.220.72:5005 или порт 5006**
2. Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

**$ cat myscript**  
**#!/bin/bash**  
**cd d3**  
**mkdir folder1 folder2 folder3**  
**cd folder1**  
**touch 1.txt 2.txt 3.txt 4.json 5.json**  
**mkdir f1 f2 f3**  
**ls -la**  
**mv 1.txt 2.txt ../**

***Чтобы выполнить скрипт в указанной оболочке, нужно установить для него флаг исполняемости:***

chmod ugo+x script.sh

***Запуск скрипта sh в linux:***

./script.sh
