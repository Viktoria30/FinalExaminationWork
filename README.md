# Условия задачи

Написать программу, которая из имеющегося массива строк формирует 
массив из строк, длинна которых меньше или равна 3 символам.
Первоначальный массив можно ввести с клавиатуры, либо задать на старте
выполнения алгоритма. При решении не рекомендуется пользоваться коллекциями,
лучше обойтись исключительно массивами.
## Примеры:
["hello", "2", "world", ":-)"] -> ["2", ":-)"]

["1234", "1567", "-2", "computer science"] -> ["-2"]

["Russia", "Denmark", "Kazan"] -> [ ]

# Текстовое описание решения задачи

1. Приглашаем пользователя ко вводу строкового массива.
2. Создаём строковый массив **array1**, далее считываем данные из терминала и сразу вносим их в массив **array1**.
3. Создадим ещё один строковый массив **array2** с длинной равной массиву **array1**.
4. Создадим целочисленный счётчик **count** для сохранения результатов условия по порядку.
5. Заходим в цикл **for** и обращаемся к первому элементу массива **array1**.
6. Заходим в условие **if** и если условие соблюдено, данный элемент состоит из 3 или менее индексов, то проваливаемся в условие и записываем этот элемент в массив **array2** с индексом 0. Если условие не соблюдается то переходим к следующему элементу массива.
7. К счётчику **count** прибавляем один.
8. Далее мы снова проходим по пунктам 5, 6, 7 пока не закончится массив **array1**.
9. Создаём метод **PrintArray** и снова проходимся по всем элементам массива **array2** чтобы показать все элементы по прядку в терминале.