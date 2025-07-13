# Лабораторная работа №1

Для начала устанвливаем ssh-ключи. Для этого вводим в терминал команду `ssh-keygen` и выбираем файл `id_rsa.pub`, чтобы сохранить туда ключ.

![telegram-cloud-photo-size-2-5415976077362326727-y](https://github.com/user-attachments/assets/d7258396-3623-4c99-9e29-f59587c31af1)

С помощью команды cat открываем содержимое файла и копируем ключ.

![telegram-cloud-photo-size-2-5415976077362326764-y](https://github.com/user-attachments/assets/c12905de-ad93-499d-a77a-c9251acb55f1)

Затем загружаем ключ в поле SSH keys на GitHub.

![telegram-cloud-photo-size-2-5415976077362326767-x](https://github.com/user-attachments/assets/a8ed5dae-7c9f-4456-8cf5-ad50cad97a50)

Теперь клонируем репозиторий с лабой к себе на компьютер. Видим успешную загрузку.

![telegram-cloud-photo-size-2-5415710279016247736-x](https://github.com/user-attachments/assets/805de09c-eb02-4180-a183-887a0094aabf)

Создаём новый файл с именем `script.bash` с помощью команды `touch`. Далее используем команду `gedit` для редактирования. Вписываем в открывшийся файл скрипт:
```
#!/bin/bash

echo "Welcome to ITMO University"
```
Сохраняем файл и запускаем скрипт с помощью комнады `bash script.bash`. Видим, что в терминале отображается нужная нам строка.

![telegram-cloud-photo-size-2-5415976077362326787-x](https://github.com/user-attachments/assets/642105d4-15d8-401d-a17a-9496529e6649)
![telegram-cloud-photo-size-2-5418227877176012385-x](https://github.com/user-attachments/assets/7d97e134-5b4d-4ee6-ae16-caa6d9042a40)

Теперь уже решаем основную задачу. В файле я ввожу следующий скрипт:
```
#!/bin/bash

echo "Welcome, $@"
```
`$@` используется для получения списка всех аргументов, которые передаются скрипту. Это помогает обрабатывать сложные имена из нескольких слов. Проверяем и видим, что всё работает как нужно.

![telegram-cloud-photo-size-2-5415955036317560537-y](https://github.com/user-attachments/assets/e4e4288e-3642-40a9-a40f-d64d800d5b0b)
![telegram-cloud-photo-size-2-5415976077362326810-x](https://github.com/user-attachments/assets/5adc6d44-910e-46b2-a7d7-9944c4203a0f)

Теперь копируем созданный файл в свой репозиторий на GitHub и оставляем коммит. Для этого вводим следующие команды:
```
git add script.bash
git commit -m "I did the first task!"
git push origin main
```
Также меня попросили ввести почту и имя пользователя.

![telegram-cloud-photo-size-2-5415955036317560586-y](https://github.com/user-attachments/assets/737965d1-d494-46e1-8fe2-ae1ab766470a)

Наш файл правильно загрузился, а значит, задание выполнено. 
