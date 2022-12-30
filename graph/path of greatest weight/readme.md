## PathFinder
Найти v-w путь в сети с неотрицательными весами, решающий задачу о пути наибольшего веса, где вес пути равен сумме <br>
весов дуг. <br>
Метод решения: алгоритм построения пути в бесконтурной сети

# Файл входных данных
 Сеть, заданная списками СЛЕД[]. <br>
N - количество вершин. <br>
Далее последовательно расположены списки последующих для каждой  вершины.  В список заносится номер вершины и вес дуги. <br>
Список заканчивается 0 (ВНИМАНИЕ! не путать с нулевым весом). В конце файла записаны источник и цель.

#Пример.
 Для сети
    
         25
      1 ---> 2      4
      |      ^      ^
     4|      |0     |7
      +----> 3 -----+

 файл данных должен быть следующим:

     4
     2  25   3   4   0
     0
     2   0   4   7   0
     0
     1
     4
  
# Файл выходных данных
В случае  отсутствия пути в файл результатов необходимо записать "N", <br>
при наличии пути - "Y" и далее с новой строки весь путь. <br>
Путь начинается источником и заканчивается целью. <br>
Узлы отделяются друг от друга пробелами, вес пути вычисляется как сумма весов всех дуг, входящих в него и записыва- <br>
ется в третьей строке. <br>
 
 Для примера, приведенного в описании файла исходных данных, файл результатов должен быть следующим:
    
    N