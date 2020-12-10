# Домашнее задание по ТРАД
Выполнил Кревский Михаил.

В этой работе я использовал и сравнил три бинарных классификатора: стандартный алгоритм на "генераторах"; модифицированный алгоритм на "генераторах", основывающийся на поиске максимально похожего элемента в обучающей выборке; стандартный классификатор - решающее дерево.

## Данные
В качестве данных я использовал классический набор с соревнования "Titanic: Machine Learning from Disaster" https://www.kaggle.com/c/titanic. Подробнее данные описаны в файле с самой работой в формате .ipynb
В ходе предобработки данных потребовалось избавться от пропусков и бинаризовать получившийся датасет. Для эффективной бинаризации потребовалось визуализировать некоторые числовые признаки, чтобы разделить их значения на диапазоны. Графики в github не отображаются, если их понадобится посмотреть, это можно сделать локально на компьютере.

## Результаты применения классификаторов

Метрика        | Базовый алгоритм | Модифицированный алгоритм | Решающее дерево |
-------------- | ---------------- | ------------------------- |---------------- |
Accuracy       |  63.0            |                     69.0  | 73.1            |
Precision      |  96.4            |                     76.4  | 66.7            |
Recall         |  21.4            |                     39.9  | 31.6            |
TNR            |  99.0            |                     83.0  | 81.3            |
NPV            |  57.6            |                     64.8  | 76.5            |
FPR            |  1.0             |                     17.0  | 18.8            |
FDR            |  3.6             |                     23.6  | 33.3            |

Можно сделать вывод, что реализованные в работе алгоритмы показывают результат на уровне стандартного решающего дерева 
