# Репозиторий для **pull request**
* В своём аккаунте на GitHub создать копию репозитория **"AndreyBulgakov19/SCV_GitPR"** с помощью кнопки **"Fork"**.
---
* Клонировать копию репозитория на локальный компьютер.
---
* Создать новую ветку.
---
* Добавить файл с инструкцией в новую ветку.
---
* Дополнить инструкцию разделами по работе с удалёнными репозиториями, pull request.
---
* Зафиксировать изменения (коммиты).
---
* Отправить изменения на GitHub.
---
* На сайте GitHub выполнить **Pull request**.
---
# Работа с Git
## 1. Проверка наличия установленного Git
В терминале выполнить команду `git version`. Если Git установлен, появится сообщение о версии программы, иначе будет сообщение об ошибке.

## 2. Установка Git
Загружаем последнюю версию программы с [сайта](http://git-scm.com/downloads).
Устанавливаем с настройками по умолчанию.

## 3. Настройка Git
Необходимо "представиться" системе контроля версий. Для этого в терминале нужно ввести 2 команды:
* git config --global user.name «Ваше имя английскими буквами»

* git config --global user.email ваша почта@example.com

## 4. Инициализация репозитория
Создаем папку. Далее открываем её в программе VS Code. Создаем файл с расширением `.md`. 
Например, `Example.md`.
Затем вводим команду `git init`.
## 5. Запись изменений в репозиторий
Для сохранения изменений вводим команду **git add название файла**  затем **git commit -m "Добавляем комментарий к действию "**
## 6.Просмотр истории коммитов
Для просмотра коммитов, необходимо воспользоваться командой **git log**. Все коммиты появятся в терминале по очередности их создания с описанием
## 7. Перемещение между сохранениями (комитами)
Для перемещения между коммитами воспользумся командой __git checkout 4 *начальные цифры нужного коммита*__
## 8. Игонорирование файлов 
Для того, чтобы исключить из отслеживания определенные файлы и папки, необходимо создать файл ***.gitignore*** и записать в него их названия илии шаблоны, соответсвующие таким файлам или папкам.
## 9. Создание веток в Git
По умолчанию имя основной ветки в Git - **master**.
Создать ветку можно командой: 
``` bash
git branch <имя новой ветки>
```
## 10. Слияние веток и разрешение конфликта 
Слияние веток выполняется командой `git merge название сливаемой ветки`.
Данная команда выполняется из той ветки, куда необходимо внести изменения.
При этом может возникнуть конфликт, для его разрешения необходимо выбрать одну из данных комманд:
![фотоинструкция](Screenshot_1.png)
## 11. Удаление веток
Для удаление ветки воспользуемся кокококомандой `git branch -d название ветки`



---
# ***Работа с удаленными репозиториями***

1. Создать аккаунт на [GitHub](https://github.com/)
2. Создать локальный репозиторий в Git см. пункт 4 "Инициализация репозитория"
3. Создать удаленный репозиторий через "+" на сайте [GitHub](https://github.com/)

*При работе с чужим удаленным репозиторием, создаем копию данного репозитория в своем аккаунте. Для этого на странице создателя  нажимаем кнопку "fork" и копируем ссылку на свою копию репозитория.*

Копируем ссылку на реппозиторий в своем аккаунте под кнопкой "Code"

4. Связать локальный репозиторий с удаленным поочередным выполнением следующих команд:
git remote add origin *ссылка на удаленный репозиторий*
git branch -M main
git push -u origin main

 *При работе с чужим удаленным репозиторием, вводим в терминал команду `git clone ссылка на удаленный репозиторий`. Создаем новую ветку и все изменения выполняем в ней*
 
5. Получить изменения из удаленного репозитория и выполнить слияние с локальной версией:
```bash
git pull
```
6. Отправить изменения из локального репозитория на удаленный и выполнить слияние:
```bash
git push
```
7. Получить список связанных репозиториев можно при помощи команды `git remote`
8. 8. Отправляем изменения автору на рассмотрение. Для этого необходимо на Github
