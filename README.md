# bash-training
1. Напишите Bash-скрипт, который будет создавать резервные копии всех файлов с заданным расширением в указанной папке. Скрипт должен выполнять следующие шаги:

* Запрашивать у пользователя путь к целевой папке, например: "/путь/к/папке".
* Запрашивать расширение файлов, которые нужно скопировать, например: ".txt".
* Создавать новую папку с текущей датой и временем, например: "резервная_копия_2023-11-05_14-30".
* Копировать все файлы с указанным расширением из целевой папки в созданную резервную папку.
* Сообщать пользователю об успешном завершении операции.
* Скрипт должен быть надежным и обрабатывать возможные ошибки, например, если указанная папка или расширение файлов не существует.

2. Подсчет количества файлов и папок в заданной папке
Напишите Bash-скрипт, который будет использовать getopts для обработки опций командной строки и циклы для обхода файлов и подсчета количества файлов и папок в заданной папке. Скрипт должен иметь следующий функционал:

Скрипт должен принимать опции командной строки:
* -p <путь>: Указывает путь к целевой папке для подсчета.
* -f: Если указана эта опция, скрипт должен подсчитывать только файлы (не папки).
* -d: Если указана эта опция, скрипт должен подсчитывать только папки (не файлы).

Скрипт должен выводить количество файлов и/или папок, в зависимости от указанных опций, в следующем формате:

* "В указанной папке <путь> найдено <количество> файлов."
* "В указанной папке <путь> найдено <количество> папок."

Пример использования скрипта:

```bash
Copy code
./count_files.sh -p /путь/к/папке
./count_files.sh -p /путь/к/папке -f
./count_files.sh -p /путь/к/папке -d
```
Скрипт должен быть способен обрабатывать возможные ошибки, такие как указание несуществующей папки, некорректные опции или отсутствие опции -d.
