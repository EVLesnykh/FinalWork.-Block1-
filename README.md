# Итоговая проверочная работа

## Задача:
Написать программу, которая из имеющегося массива строк формирует массив из строк, длина 
которых либо меньше либо равна 3 символа. Первоначальный массив можно ввести с клавиатуры, 
либо задать на старте выполнения алгоритма. При решение не рекомендуется пользоваться коллекциями, лучше обойтись исключительно массивами.

### Примеры:
* ["hello", "2", "world", ":-)"] -> ["2", ":-)"]
* ["1234", "1567", "-2", "computer science"] -> ["-2"]
* ["Russia", "Denmark", "Kazan"] -> []

### ***Примечание:***              
#### Для выполнения проверочной работы необходимо:
1. Создать репозиторий на GitHub.
2. Нарисовать блок-схему алгоритма.
3. Снабдить репозиторий оформленным текстовым описанием решения (файл README.md).
4. Написать программу, решающую поставленную задачу.
5. Использовать контроль версий в работе над этим проектом.

## Описание алгоритма решения задачи:
1. Задаем исходный массив строк originalArray, где элементы массива инициализируем сразу же после объявления массива;
2. Также создаем вспомогательный массив строк newArray, куда будут записываться отсортированные значения, согласно заданному условию в цикле(длина элемента массива <= 3 символа);
3. Инициализируем вспомогательную переменную count = 0, в которую запишем количество элементов массива, длина которых <=3 символа;
4. Создаем метод void ResultArray, который позволяет сформировать массив newArray, состоящий из элементов, длина которых <=3 символа. 
 _В теле метода для инициализации цикла используем оператор for. Далее делаем перебор значений из исходного массива originalArray на соответствие условию: длина символов <=3. Если элемент массива удовлетворяет условию кладем значение в новый массив newArray, повторяем до тех пор пока не достигнем конца исходного массива. Иначе если уловие не выполнено выводим пустую строку._

5. Создаем метод void PrintArray, который позволяет вывести полученный результат на экран.

6. На экран выводим исходный массив и новый массив, полученный согласно заданному условию.