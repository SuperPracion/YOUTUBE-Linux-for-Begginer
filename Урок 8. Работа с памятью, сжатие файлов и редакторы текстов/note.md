## Урок 8. Работа с памятью, сжатие файлов и редакторы текстов 
### [Ссылка на урок](https://www.youtube.com/watch?v=pZacw30UI90)

### gedit
    Стандартный текстовый редактор с графическим интерфейсом

### top
    Консольная утилита (table of processes) выводящая в консоль информацию о запущенных процессах в системе. По умолчанию сортируется по нагрузки на ЦП

| Атрибут | Описание |
|---------|----------|
| PID     | уникальный идентификатор процесса|
| USER    | (USERNAME) пользователь от имени кого был запущен процесс|
| PR      | (PRIORITY) текущий приоритет процесса|
| NI      | (NICE) приоритет процесса выставленный командой nic|
| VIRT    | полный объём занимаемый памяти процессом|
| RES     | текущее использование ОЗУ|
| SHR     | ?|
| S       | ?|
| %CPU    | процент от занимаемого процессорного времени|
| %MEM    | процент от занимаемый памяти относительно полного объёма|
| TIME+   | время работы процесса|
| COMMAND | команды запустившая процесс|

### ps
    Утилита командной строки, выводящая информацию о запущенных процессах 

| Атрибут | Описание |
|---------|----------|
|-aux     |(all users executable) выводит информацию о всех запущенных процессах, всех пользователей|
| \|      |указывает на связку с другой командной фильтрации, например фильтрация текста grep|
    

### free
    Утилита командной строки, выводящая информацию об используемой памяти

|  Атрибут | Описание |
|----------|----------|
| total    | всего памяти|
| used     | используемая память|
| free     | свободная память|
| shared   | общая|
| buff/cash| объединённая память используемая ядром|
| available| доступно памяти|
| -h       | вывод информации в удобной для человека виде|


### tree
    Утилита командной строки, выводящая информацию о файлах и директориях в древовидном формате


### tar
    Формат битового потока, использующий в сегодняшнее время дни для архивации нескольких файлов в один и подготовке к компрессии других форматов, folder -> folder.tar

| Атрибут | Описание |
|---------|----------|
| cf      | (create folder) позволяет преобразовать директорию с архив с форматом folder - > folder.tar|
| tf      | (test folder) позволяет просмотреть содержимое архива с форматом .tar|
| xf      | (execute folder) - выполняет процесс разархивации архива в формате folder.tar -> folder|
| x**v**f | (view) аналогичен xf, но с выводом в поток информации о процессе|


### zip
    Утилита позволяющая преобразовывать файлы без дополнительной подготовки.  
    -r - флаг для архивации folder -> folder.zip

| Атрибут | Описание |
|---------|----------|
| unzip   |запускает процесс разархивации архива folder.zip -> folder|



### xz 
    Утилита семейства Unix, сжимает данные с высокой степенью компрессии. Использует алгоритм lzma2. Для архивации требуется подготовленный архив в формате tar.
    unxz - запускает процесс разархивации архива в формате xz. folder.tar.xz -> folder.tar


### gzip
    Утилита семейства Unix, выполняющая сжатие и восстановление по алгоритму Deflate. Для архивации требуется подготовленный архив в формате tar. folder.tar -> folder.tar.gzip

| Атрибут | Описание |
|---------|----------|
| -d      |  запускает процесс разархивации. folder.tar.grip -> folder.tar|
| -9      | запускает процесс сильнейшей архивации|
| -1      | запускает процесс быстрейшей архивации|

 
### bzip2
    Утилита семейства Unix, выполняющая сжатие и восстановление алгоритмом bzip2, является **лучшим** для архивации, чем gzip или zip. Для архивации требуется подготовленный архив в формате tar.


