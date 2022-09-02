1. Посмотреть, где я: 
 
 ``` javascript
pwd
```

2. Создать папку: 
``` javascript
mkdir qa_sts
```

3. Зайти в папку: 
``` javascript
cd qa_sts
```
4. Создать 3 папки: 
``` javascript
mkdir qa_1 qa_2 qa_3
```
5. Зайти в любую папку: 
``` javascript
cd qa_1
```
6. Создать 5 файлов: 
``` javascript
cat>sts1.txt sts2.txt sts3.txt sts1.json sts2.json
```
7. Создать 3 папки: 
``` javascript
mkdir qa1_1 qa1_2 qa1_3
```
8. Вывести список содержимого папки: 
``` javascript
ls -la
```
9. Открыть любой txt файл: 
``` javascript
vim sts1.txt
```
10. Написать туда любой текст: 
ввод данных в режиме редактирования

11.  Сохранить и выйти: 
``` javascript
Esc + :wq
```
12. Выйти из папки на уровень выше: 
``` javascript
cd ..
```
13. Переместить любые 2 файла, которые вы создали, в любую другую папку: 
``` javascript
mv qa1_1/{sts1.txt,sts1.json} qa1_2
```
14. Скопировать любые 2 файла, которые вы создали, в любую другую папку:
``` javascript
cp qa1_2/{sts1.txt,sts1.json} qa1_3
```

15. Найти файл по имени: 
``` javascript
find . -name sts1.txt
```

16. Посмотреть содержимое в реальном времени:
``` javascript
tail -f sts1.txt
```
17. Вывести несколько первых строк из текстового файла:
``` javascript
head -n2 sts1.txt
```
18. Вывести несколько последних строк из текстового файла: 
``` javascript
tail -n4 sts1.txt
```
19. Посмотреть содержимое длинного файла:
``` javascript
less sts1.txt
```
20. Вывести дату и время:
``` javascript
date
```
Задание*
1. Отправить http запрос на сервер:
``` javascript
curl  "http://162.55.220.72:5005/get_method?name=arina&age=twenty_two"
```
2. Написать скрипт, который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13:
``` javascript
vim commands.sh

#!/bin/bash
mkdir qa2_sts
cd qa2_sts
mkdir qa_1 qa_2 qa_3
cd qa_1
cat> sts1.txt sts2.txt sts3.txt sts1.json sts2.json
mkdir qa1_1 qa1_2 qa1_3
ls -la
cd ..
mv qa_1/sts1.txt qa_2/sts1.txt
mv qa1_1/sts2.txt qa1_2/sts2.txt
```