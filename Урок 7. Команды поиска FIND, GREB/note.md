## Урок 7. Команды поиска FIND, GREP
### [Ссылка на урок](https://www.youtube.com/watch?v=IjgwSbdjYKs)

| Команда | Описание | Атрибут | Описание атрибута |
|---------|----------|---------|-------------------|
| sort    | утилита семейства UNIX, сортирующая стандартный вывод| | |
|         |          | -n      | атрибут необходимый для корректной работы сортировки чисел|
| cat     | последовательно считывать данные и выводить их в стандартный вывод | | |
| grep    | выполняющая поиск совпадения в файлах | | |
| |                  | -n      | дополнительно указывает номер строки|
| |                  | -i      | игнорирование регистра|
| find    | выполняющая поиск файлом или каталогов| | |
| |                  | .       | атрибут указывающий на текущий каталог (можно упустить)|
| |                  | -type   | f - файл, d - каталог указывает на искомый тип|
| |                  | -name   | производит поиск по переданному шаблону имени|
| |                  | -iname  | аналогичен name, но с игнорированием регистра|
| |                  | -perm   | производить поиск по правам|
| |                  | -size   | производит поиск по размеру, + размер должен быть больше n, - размер должен быть меньше n|
| |                  | -not    | используется когда необходимо найти всё остальное, кроме указанного|

<!---
find - утилита UNIX семейства, выполняющая поиск файлом или каталогов по переданному имени
Используется в UNIX-подобный ОС. По умолчанию find производит поиск в рабочем каталоге.

. - атрибут указывающий на текущий каталог (можно упустить)

-type - указывает на искомый тип 
    f - файл
    d - каталог

-name - производит поиск по переданному шаблону имени

-iname - аналогичен name, но с игнорированием регистра

-perm - производить поиск по правам

-size - производит поиск по размеру
    + - указывает на то, что размер должен быть больше n 
    - - указывает на то, что размер должен быть меньше n

-not - используется когда необходимо найти всё остальное, кроме указанного


grep - утилита UNIX семейства, выполняющая поиск совпадения в файлах
-n при выводе дополнительно указывает номер строки, в которой нашлось совпадение
-i игнорирование регистра

cat - утилита семейства UNIX, позволяющая последовательно считывать данные и выводить их в стандартный вывод
(стандартным выводом может быть, как терминал, так и другой файл)

sort - утилита семейства UNIX, сортирующая стандартный вывод|
-->