Втора лабораториска вежба по Софтверско инженерство

Петар Лазаровски, 183052

Група на код:

Control Flow Graph

![Control Flow Graph](https://user-images.githubusercontent.com/82048002/119946021-7098e500-bf96-11eb-9ece-c5cbc6a10818.png)

Цикломатска комплексност

Цикломатската комплексност на овој код е 8, истата ја добив преку формулата E-V+2, каде што P е бројот на предикатни јазли. Во случајoв E = 26, V = 20, па цикломатската комплексност изнесува 8.

Тест случаи според критериумот Every statement

- if(hr<0 || hr>24)
   hr < 0 || x (hr=-5 min=15 sec=15)
   hr > 0 && hr>24 (hr=30 min=8 sec=8)
   hr>0 && hr <24 (hr=11 min=10 sec=10)
- if(min<0 || min>59)
   min < 0 || x (hr=12 min =-15 sec=12)
   min > 59 (hr=15 min=60 sec=11)
   min>0 && min<59 (hr=14 min=15 sec=35)
- if(sec>=0 && sec<=59)
   sec>=0 && sec<=59 (hr=10 min=10 sec=30)
   sec>=59 (hr=19 min=15 sec=60)
   sec<=0 || x (hr=19 min=10 sec=-20)
- else if(hr==24 && min==0 && sec==0)
   hr==24 && min==0 && sec==0 (hr=24 min=0 sec=0)
   hr==24 && min!=0 || x (hr=24 min=37 sec=24)
   hr==24 && min==0 && sec!=0 (hr=24 min=0 sec=35)
   hr!=24 || x (hr=5 min=24 sec=24) 

Тест случаи според критериумот Every path

![ЕveryBranch](https://user-images.githubusercontent.com/82048002/119946370-db4a2080-bf96-11eb-9846-a9564bb50330.png)

Објаснување на напишаните unit tests
... ...
