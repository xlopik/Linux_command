grep - утилита поиск в файле, поиска строк, соответствующих строке в тексте или содержимому файлов. regexp задает шаблон для поиска текста.Они регистрзависмы.
Пример:
1- точное совпадение встроено
2- вкл шаблон поиска : точка ( .) пример Regex: grep \.txt рез- file.txt (\. - именно точку ищем), несколько точки ва..я-васия 
3- допустимые : А[нл][нл]а - Анна [А-Яа-яЁё]  — все русские буквы (только диапазон [1-31]от 1-3)
4- ^ - такая хуембула : [^0-9]  — любой символ, кроме цифр [^а-в8]  — любой символ, кроме букв «а», «б», «в» и цифры 8
5 - экранирование Regex: fruits\[0\] Найдет: fruits[0] , пример 0[1-9]|[12][0-9]|3[01] 0, 2 символо в 1-9 или 1 ии 2 , 2 символ от 0-9 и т.д.
6 - Одного символа — используем [] Нескольких символов или целого слова — используем | cat y.y | grep  'ва(с|си)я' вывод - вася ,васия
Мета:
grep  -P '.*\d\d\.\d\d\.\d\d\d\d.' или (\d{2}\.\d{2}.\d{4})- 2 смвола цыфр, 2 и 4 ,  \w+@\w+\.\w+ - test@mail.ru 1 + - или более символов после \w * - 0 или более ? - 0 или 1
7- () - скобки это группа  квантификатор Regex: (data){2} , \1 повторение группы (Perl - $  Python group[1] PHP $matches[1])
8- Regex: \bарка\b арка - точное совпадение
9- ^ — начало текста (строки) $ — конец текста (строки) Regex: ^Я нашел!$ Я нашел!
10- Замена RegEx: (Оля) \+ Маша Замена: $1 Текст был: Оля + Маша Текст стал: Оля ,Замена даты  RegEx: (\d{2})\.(\d{2})\.(\d{4}) Замена: $3-$2-$1
https://habr.com/ru/post/545150/

root@хзхз:~# grep .ru ~/y.y
test@mail.rugfhgfhgfhfg



















du (разные опции)
df (разные опции)
find
head -n10
tail -n10
tail -f
top / htop
watch
rsync (хотя бы привести две директории к одному виду)
scp
vim / vimtutor – банально файл открывать/закрывать надо уметь
ps uaxwf (что каждая опция значит)
pstree
sort, uniq
diff
stat (что такое Access, Modify, Change?)
pgrep / pkill
dig
lsof
strace
crontab
date
touch (что конкретно делает?)
mount
iostat / iotop /
vmstat / free
git: git blame, git diff, git status, git pull, git add, git commit, git push (полезно будет, мы юзаем)
ping, traceroute, mtr, ip r, ip a, iftop
netstat, ss
telnet, netcat, netcat -u
curl, wget
time


