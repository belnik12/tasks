task1

Напишите программу, которая рассчитывает и подает на стандартный вывод следующие
значения:
 90 перцентиль
 медиана
 максимальное значение
 минимальное значение
 среднее значение
Данные для расчетов считываются из файла, путь к которому подается в виде аргумента.
Числа в файле в пределах от -32 768 до 32 767.
Каждое число с новой строки.
В файле не более 1000 строк.
Вывод значений в указанной последовательности, каждое значение заканчивается символом
новой строки.
Все значения с точностью до сотых: 2.50 2.00 0.03.
Пример
На вход:
5
8
0
0
1
5
5
5
10
6

Вывод:
8.20
5.00
10.00
0.00
4.50
-------------------------------------------------------------------

task2

Напишите программу, которая рассчитывает положение точки относительно выпуклого
четырехугольника в двумерном пространстве.
Координаты фигуры считываются из файла1. Это вершины четырехугольника, которые
располагаются в порядке обхода фигуры по часовой стрелке.
Пример:
0 0\n
0 5.5\n
5.5 5.5\n
5.5 0\n

Координаты точек считываются из файла2. 
Пример:
1.3 1.23\n
10 9\n
0 3\n
5.5 5.5\n
0 -1\n

Файлы передаются программе в качестве аргументов. Файл с координатами четырехугольника - 1
аргумент, файл с координатами точек - 2 аргумент.
Координаты в диапазоне float.
Количество точек от 1 до 100.
Вывод каждого положения точки заканчивается символом новой строки.
Соответствия ответов:
0 - точка на одной из вершин
1 - точка на одной из сторон
2 - точка внутри
3 - точка снаружи
-----------------------------------------------------------------------

task3

В магазине 5 касс, в каждый момент времени к кассе стоит очередь некоторой длины.
Каждые 30 минут измеряется средняя длина очереди в каждую кассу и для каждой кассы это
значение записывается в соответствующий ей файл (всего 5 файлов).
Каждое значение заканчивается символом новой строки.
Магазин работает 8 часов в день.
Рассматривается только один день.
На момент запуска приложения все значения уже находятся в файлах.
Написать программу, которая по данным замеров определяет интервал времени, когда в
магазине было наибольшее количество посетителей за день.
Аргумент программы - путь к каталогу с файлами. В каталоге будут 5 файлов: Cash1.txt, Cash2.txt ...
Cash5.txt.
Пример одного из файлов:
1\n
1.2\n
1.3\n
1.34\n
1.5\n
1.9\n
1.7\n
1.832\n
1.91\n
2.3\n
2.5\n
4.9\n
3.5\n
2.34\n
1.242\n
1.01\n

Выведите номер интервала, в котором было наибольшее число посетителей в очередях магазина
на всех кассах.
Первый интервал идет под номером 1, последний под номером 16.
В случае обнаружения нескольких интервалов следует выводить первый из них.
--------------------------------------------------------------------------------------

task4

В течении дня в банк заходят люди, для каждого посещения фиксируется время захода в банк и
время выхода.
Банк работает с 8:00 до 20:00.
Написать программу, которая определяет периоды времени, когда в банке было максимальное
количество посетителей.
Файл содержит информацию о времени посещения банка каждым посетителем, округленном до
минут.
Время входа посетителя меньше либо равно времени выхода.
Выведите интервалы времени, когда в банке было максимальное число посетителей.
Начало и конец интервала разделяются пробелом.
В случае необходимости вывести несколько периодов, в качестве разделителя между ними
следует использовать символ перевода строки.
Пример
На вход:
8:00 8:30\n
8:15 8:45\n
8:45 9:00\n
8:30 9:00\n
9:00 9:30\n
9:10 9:20\n

Вывод:
8:15 9:00\n
9:10 9:20\n
