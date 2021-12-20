Четвертая лабораторная https://github.com/Maerodrim/Pi_calc
Язык программирования: С/С++
IDE: VS2019
R5 4600H + GTX 1650
CPU Time
3.14169
time= 458 ms
GPU_1 Time
3.14169
time = 122.026 ms

Третья лабораторная https://github.com/Maerodrim/SAP
Язык программирования: С/С++
IDE: VS2019
В ходе	эксперемента использовался R7 3700X + RTX 3070
Time on GPU: 17.0518 ms
Так же в репозитории есть вариант исполнения медианного фильтра на Java https://github.com/Maerodrim/Client_Lab (вторая лабораторная)

Вторая лабораторная https://github.com/Maerodrim/VectorAdditionCUDA
Язык программирования: С/С++
IDE: VS2019
В ходе	эксперемента использовался R7 3700X + RTX 3070
РЕЗУЛЬТАТЫ ВЫЧИСЛЕНИЙ
Size : 1000
CPU Time: 0.002900 ms
GPU Time (improved): 0.020480 ms
Size : 10000
CPU Time: 0.027200 ms
GPU Time (improved): 0.028672 ms
Size : 100000
CPU Time: 0.258100 ms
GPU Time (improved): 0.094208 ms
Size : 1000000
CPU Time: 2.722100 ms
GPU Time (improved): 0.205824 ms
Size : 10000000
CPU Time: 27.446700 ms
GPU Time (improved): 1.721440 ms


Был написан параллельный алгоритм перемножения матриц с использованием разбиение матрицы на матрицы 16*16 и работу уже с ними + использовалась shared память. 
Алгоритм для CPU стандартный.
Язык программирования: С/С++
IDE: VS2019

В ходе	эксперемента использовалось два стенда
1)R5 4600H + GTX 1650
2)R7 3700X + RTX 3070
РЕЗУЛЬТАТЫ ВЫЧИСЛЕНИЙ

Для эксперимента были использованы матрицы, размерности которых кратны 32, чтобы загрузка блоков GPU была максимальной.
Результат эксперемента для сборки R5 4600H + GTX 1650
Experiment for matrix size: 64
Time spent executing by the CPU: 1.00 millseconds
Time spent executing by the GPU events: 0.22 millseconds
Time spent executing by the GPU: 1.00 millseconds
Acceleration factor: 1.00
Relevance: true
Experiment for matrix size: 128
Time spent executing by the CPU: 7.00 millseconds
Time spent executing by the GPU events: 0.59 millseconds
Time spent executing by the GPU: 2.00 millseconds
Acceleration factor: 3.50
Relevance: true
Experiment for matrix size: 256
Time spent executing by the CPU: 56.00 millseconds
Time spent executing by the GPU events: 1.69 millseconds
Time spent executing by the GPU: 2.00 millseconds
Acceleration factor: 28.00
Relevance: true
Experiment for matrix size: 512
Time spent executing by the CPU: 536.00 millseconds
Time spent executing by the GPU events: 11.49 millseconds
Time spent executing by the GPU: 13.00 millseconds
Acceleration factor: 41.23
Relevance: true
Experiment for matrix size: 1024
Time spent executing by the CPU: 8849.00 millseconds
Time spent executing by the GPU events: 86.66 millseconds
Time spent executing by the GPU: 89.00 millseconds
Acceleration factor: 99.43
Relevance: true
Experiment for matrix size: 2048
Time spent executing by the CPU: 171649.00 millseconds
Time spent executing by the GPU events: 524.30 millseconds
Time spent executing by the GPU: 540.00 millseconds
Acceleration factor: 317.87
Relevance: true

Результат эксперемента для сборки R7 3700X + RTX 3070
Experiment for matrix size: 64
Time spent executing by the CPU: 1.00 millseconds
Time spent executing by the GPU events: 0.20 millseconds
Time spent executing by the GPU: 0.00 millseconds
Acceleration factor: inf
Relevance: true
Experiment for matrix size: 128
Time spent executing by the CPU: 7.00 millseconds
Time spent executing by the GPU events: 0.31 millseconds
Time spent executing by the GPU: 1.00 millseconds
Acceleration factor: 7.00
Relevance: true
Experiment for matrix size: 256
Time spent executing by the CPU: 54.00 millseconds
Time spent executing by the GPU events: 0.68 millseconds
Time spent executing by the GPU: 1.00 millseconds
Acceleration factor: 54.00
Relevance: true
Experiment for matrix size: 512
Time spent executing by the CPU: 568.00 millseconds
Time spent executing by the GPU events: 3.37 millseconds
Time spent executing by the GPU: 5.00 millseconds
Acceleration factor: 113.60
Relevance: true
Experiment for matrix size: 1024
Time spent executing by the CPU: 4673.00 millseconds
Time spent executing by the GPU events: 23.46 millseconds
Time spent executing by the GPU: 25.00 millseconds
Acceleration factor: 186.92
Relevance: true
Experiment for matrix size: 2048
Time spent executing by the CPU: 48258.00 millseconds
Time spent executing by the GPU events: 177.99 millseconds
Time spent executing by the GPU: 192.00 millseconds
Acceleration factor: 251.34
Relevance: true
