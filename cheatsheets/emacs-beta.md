#вопросы Emacs
##ТЕРМИНОЛОГИЯ
1. **чем отличается текстовый редактор от текстового процессора?**
2. **какие есть варианты Emacs?**
3. **что такое буфер?**
 Буфер — объект, представляющий какой-либо текст.
4. **что такое фрейм?**
 Фрейм соответствует окну в обычном понимании этого слова (как у X Window System). Каждый фрейм содержит область вывода и одно или несколько окон Emacs.
5. **что такое окно?**
 Окно — это просто прямоугольная область фрейма, которая отображает один из буферов. Помимо этого, каждое окно имеет свою строку состояния (англ. mode line), где выводится название буфера, его основной режим и т. п.
6. **что такое область вывода**
 Область вывода (echo area) — одна или несколько (по необходимости) строк внизу фрейма, в которой Emacs выводит различные сообщения, а также запрашивает подтверждения и дополнительную информацию от пользователя.
7. **что такое минибуфер?**
 Минибуфер используется для ввода дополнительной информации. Он всегда отображается в области вывода. Это такой же буфер, как и все остальные, что даёт интересный эффект: например, при операции замены текста, можно ввести многострочный текст, что невозможно в большинстве других редакторов.
8. **на каком языке программирования написан Emacs?**
 Emacs написан на двух языках: C и Emacs Lisp

##ШПАРГАЛКИ ПО РЕДАКТОРУ
1. **Описание функции**
 ^H f <функция>
2. **На какой клавише висит функция**
 H w <функция>

##ХОЖДЕНИЕ   ПО   ФАЙЛАМ
1. **Сохранить файл**
 ^X ^S
2. **Выйти из всех файлов с сохранением**
 ^X ^C
3. **Записать файл под другим именем write-file**
 ^X ^W
4. **Список файлов в каталоге**
 ^X ^D<каталог>
5. **Просмотр файла**
 M-x view-file
6. **Вставка файла**
 M-x insert-file

##ОКНА, БУФЕРЫ
1. **Уничтожить окно**
^X 0
2. **Первое окно на весь экран**
^X 1
3. **В другое окно**
^X o
4. **Список буферов**
^X ^B
5. **kill-buffer**
^X k

##ПЕРЕМЕЩЕНИЯ   ПО   ТЕКСТУ
1. **Сдвинуться на символ вперед**
^f
2. **Сдвинуться на символ назад**
^b
3. **Сдвинуться на строку вперед**
^n
4. **Сдвинуться на строку назад**
^p
5. **На слово вперед**
M- f
6. **На слово назад**
M- b
7. **На страницу вверх**
M-V
8. **На страницу вниз**
^V
9. **В начало строки**
^A
10. **В конец строки**
^E

##РЕДАКТИРОВАНИЕ СТРОКИ
1. **Удалить символ**
^D
2. **Удалить слово и пробелы за ним**
M-d

##МАКРОКОМАНДЫ
1. **Выполнить функцию по имени**
M-x <функция>
2. **Установить значение переменной**
M-x set-variable
3. **Повесить на клавишу функцию.**
M-x global-set-key  <функция>

##КОМАНДЫ МИНИБУФЕРА
1. **Повторить последнюю команду**
^X
2. **История команд**
M-x
3. **Дополнить**
Tab

##ПРОЧЕЕ
1. **Выйти в ОС**
[^X] ^Z
2. **Выполнить команду shell по запросу**
ESC !
3. **Загрузить файл с ЛИСПОМ  .elc, .el**
M-x load-file

##ВКУСНЯШКИ
1. **Психотерапевт. Психотерап. сеанс. Пирамидка**
M-x doctor psy hanoi
2. **Календарь**
M-x calendar

###дополнительно
- [все команды](http://lib.ru/unixhelp/emacs.txt)