## Урок 5. Работа с файлами и директориями
### [Ссылка на урок](https://www.youtube.com/watch?v=jifzdBvUmEs)


| Команда | Расшифровка                        | Описание                      | Аргумент | Описание |
|---------|------------------------------------|-------------------------------|----------|----------|
||||||
| touch |                | позволяет создавать файлы | имя.расширение | необходимо указать имя и расширение для создаваемого файла | 
| nano  |                | утилита позволяющая просматривать/редактировать/сохранять информацию в файл | имя-файла | указывается поле вызова команды |
| mkdir | **m**a**k**e **dir**ectory | создаёт каталог с указанным именем| имя[имя]| создаёт каталог с указанным именем. позволяет создать несколько, перечисляя их через пробел|
| cp    | **c**o**p**y   | копирует выбранный файл/каталог в указанное место | путь-от-источника/путь-до-назначения |                                                         |
| mv    | **m**o**v**e   | перемещает источник от указанного места в место назначение| путь-от-источника/путь-до-назначения|                                                  |
| rm    | **r**e**m**ove | удаляет источник. по умолчанию работает только с удалением файлов, но не директорий |     |                                                        |
|||                                                                                                            | -r  | рекурсивное удаление. позволяет удалять каталоги       |
|||                                                                                                            | -f  | игнорирование несущ. файлов                            |
|||                                                                                                            | -rf | удаление директорий игнорируя файлы и возможные ошибки |
| sudo   | **s**ubstitute **u**ser and **do** | дословно означает: подменить пользователя и выполнить.|||
||                                            | Основная идея - дать пользователем минимальный доступ для решения поставленных задач|||
|||                                                                                                   | !!     | выполнить предыдущую команду от имени суперпользователя |
|||                                                                                                   | -s     | позволяет запустить командный интерпретатор|
|||                                                                                                   | -**u** | позволяет указать, от имени какого пользователя нужно выполнять программу. |
|||                                                                                                   | -su    | интерпретатор + текущий пользователь|
| chown | **ch**ange **own**er | изменять владельца и группу. требуется sudo                                     | owner:group | необходимо указать два имени |
| chmod | **ch**ange **mod**e  | изменяет права на файл для администратора, группы и пользователей. требуется sudo| xxx         | 7 - rwx, 6 - rw, 4 - r  |