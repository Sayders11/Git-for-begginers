# Базовые команды

## Навигация в системе

- ``` pwd ``` - показывает текущую директорию

- ``` ls ``` - показывает содержимое текущий директории

- ``` ls -a ``` - то же самое + скрытые файлы

- ``` cd ``` - эта команда перемещает нас в другую папку, соответственно, после неё нужно написать название папки, в которую перемещаемся.Допускается переходить сразу на несколько уровней, например, ``` cd dev/test-project/info ```

- ``` cd .. ``` - вернуться на уровень выше

- ``` cd ~ ``` - вернуться в домашнюю директорию, для Windows это /Users/Username

- ``` cd / ``` - перейти в корневую директорию

# Работа с файлами и папками

## Создание

``` touch readme.txt ``` - создать файл ``` readme.txt ``` в текущей папке. Допускается создание сразу нескольких файлов, например, ``` touch README.md style.css script.js ```

``` mkdir project ``` - создать новую директорию (папку) с именем ``` project``` в текущей папке

## Копирование и перемещение

``` cp file.txt ~/my-dir ``` - скопирует файл в другое место

``` mv file.txt ~/my-dir ``` - переместит файл

## Чтение

``` cat README.md ``` - распечатает содержимое файла в консоли

``` pbcopy < README.md ``` - копировать содержимое файла в буфер

## Удаление

``` rm readme.txt ``` - удалить файл

``` rmdir project ``` - удалить папку/директорию (только если она пуста)

``` rm -r project ``` - рекурсия, удаляет сначала всё содержимое папки, а затем саму папку (иначе нужно ручками)


## Прочие ништяки

- Команды можно объединять двумя амперсандами ``` && ```. Например, ``` mkdir dev && cd dev && touch README.md ```


# Git'ование

## Как создать репу

``` git init ``` - инициализация локального репозитория

``` git add text.txt ``` - добавление файлов к коммиту

``` git commit -m "Мой первый коммит" ``` - для коммита, после добавления

``` git push ``` - окончательно запушить коммит на гитхаб


``` rm -rf .git ``` - разгитить папку (вдруг пригодится)
// ``` -r ``` - рекурсия, ``` -f ``` - forced


``` git status ``` - проверить состояние репы

``` git log ``` - чекнуть логи репы


# Генерация SSH-ключа

## ключ ``` .pub ``` - публичный, второй - персональный

- сначала стоит проверить наличие ключа командой ``` ls -la .ssh/ ```

``` ssh-keygen -t ed25519 -C "tvoi email" ``` - генерируем ключ

``` ssh-keygen -t rsa -b 4096 -C "email" ``` - альтернативный вариант шифрования ключа

- кодовую фразу для ключа можно не устанавливать и оставить пустой








 
