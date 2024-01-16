# Реализация бинарного дерева поиска на языке Python

## Содержание

**Этот файл содержит реализацию бинарного дерева поиска на языке Python. Класс Node представляет узел дерева, а класс Tree предоставляет методы для работы с деревом.**

## Описание работы
Класс Node имеет атрибуты `data`, `left` и `right`, которые хранят значение данных узла, ссылки на левого и правого потомков соответственно. Конструктор класса `Node` принимает значение данных в качестве аргумента и инициализирует атрибуты `left` и `right` значением None.

Класс **Tree** имеет атрибут `root`, который хранит ссылку на корневой узел дерева. Конструктор класса **Tree** инициализирует атрибут `root` значением `None`.

Метод append класса **Tree** добавляет новый узел с заданным значением данных в дерево. Если дерево пустое, то корневой узел будет равен новому узлу. В противном случае метод выполняет рекурсивный обход дерева, чтобы найти место для добавления нового узла. 

*Если значение данных меньше значения корневого узла, то новый узел будет добавлен в левое поддерево. Если значение данных больше значения корневого узла, то новый узел будет добавлен в правое поддерево.*

Метод `show_tree` класса **Tree** рекурсивно выводит дерево в консоль. Если узел равен `None`, то метод завершает обход дерева. В противном случае метод вызывает себя для левого и правого поддеревьев, а затем выводит значение данных текущего узла.

В конце файла приведен пример использования класса **Tree**. Создается экземпляр класса **Tree**, и для каждого значения из последовательности `binary_line` создается новый узел и добавляется в дерево. Затем вызывается метод show_tree для вывода дерева на экран.



### Обратите внимание, что данный код предоставляет только реализацию базового функционала бинарного дерева поиска. Для полноценного использования дерева вам может потребоваться дополнительная функциональность, такая как поиск узла, удаление узла и т.д.