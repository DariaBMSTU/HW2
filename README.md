# HW2
В аргументе командной строки передаётся имя текстового файла (файлов – задача а), в котором записана двумерная матрица (матрицы – задача а) вещественных чисел. Необходимо напечатать на стандартный выходной поток результат транспонирования матрицы во входном файле

Формат хранения матрицы (матриц) в файле: 
Разреженный – в первой строке файла записано количество строк матрицы; во второй - количество столбцов матрицы; в третьей - количество ненулевых элементов матрицы; в последующих строках файла записаны индексы и значения этих ненулевых элементов матрицы (информация о каждом элементе матрицы записана на отдельной строке) в следующей последовательности: номер_строки номер_столбца значение_элемента. Считать, что пары индексов элементов матрицы в файле упорядочены по возрастанию.

В качестве внутреннего представления матрицы в памяти программы использовать: Двумерный массив вещественных чисел

Требование к реализации для всех вариантов: целевой алгоритм не должен зависеть от представления матрицы в файле и в памяти, т.е. для работы с матрицей должны быть реализованы и использованы в алгоритме функции: double get_elem(void *matr, int row, int col), которая возвращает значение элемента матрицы по его индексам, и void set_elem(void*matr, int row, int col, double elem), которая устанавливает значение элемента матрицы по его индексам
