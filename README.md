# Laba2
# Лабораторная работа №2. Обнаружение и исправление ошибок
Работу выполнила Беляева Дарья БИ-41
## 1. Изучение исходного кода
Был проведен анализ исходного кода и Модификации битов. Был разработан способ модификации бита, заключающийся в замене его на противоположное значение случайного бита.
## 2. Исследование XOR-суммы
XOR-сумма является одним из способов проверки данных при их передаче. Однако, если два байта поменяются местами, то XOR-сумма не заметит этого изменения. В ходе изучения XOR-суммы было установлено, что модификация битов может вызвать дополнительные изменения в XOR-сумме. Это свойство может быть использовано для устранения ошибок при передаче данных, так как любая модификация данных приводит к модификации XOR-суммы.
## 3. Исследование обнаруживающих способностей
Для исследования аобнаруживающей способности было проведено 2^ экспериментов, в процессе изменения печени которых от 1 до 32 битов.

Ниже представлена ​​таблица, отображающая количество модифицированных битов, количество проведенных экспериментов, а также количество успешно определенных преобразований данных различными алгоритмами расчета контрольной суммы.
| № Бита | Н | ИСКЛЮЧАЮЩЕЕ ИЛИ | CRC16 | CRC32 |
| ---------- | ---------- | ---------- | ---------- | ---------- |
  | 1 |     24 |      0 |      0 |      0 |
  | 2 |    276 |     24 |      0 |      0 |
  | 3 |   2024 |      0 |      0 |      0 |
  | 4 | 10626 |    252 |      8 |      0 |
  | 5 | 42504 |      0 |      0 |      0 |
  | 6 | 134596 |   1512 |      8 |      0 |
  | 7 | 346104 |      0 |      0 |      0 |
  | 8 | 735471 |   5670 |     30 |      0 |
  | 9 | 1307504 |      0 |      0 |      0 |
  | 10 | 1961256 | 13608 |     41 |      0 |
  | 11 | 2496144 |      0 |      0 |      0 |
  | 12 | 2704156 | 20412 |     64 |      0 |
  | 13 | 2496144 |      0 |      0 |      0 |
  | 14 | 1961256 | 17496 |     58 |      0 |
  | 15 | 1307504 |      0 |      0 |      0 |
  | 16 | 735471 |   6561 |     33 |      0 |
  | 17 | 346104 |      0 |      0 |      0 |
  | 18 | 134596 |      0 |     13 |      0 |
  | 19 | 42504 |      0 |      0 |      0 |
  | 20 | 10626 |      0 |      0 |      0 |
   | 21 |   2024 |      0 |      0 |      0 |
   | 22 |    276 |      0 |      0 |      0 |
   | 23 |     24 |      0 |      0 |      0 |
   | 24 |      1 |      0 |      0 |      0 |
   | 25 |      0 |     0 |      0 |      0 |
   | 26 |      0 |      0 |      0 |     0 |
   | 27 |      0 |      0 |      0 |      0 |
   | 28 |      0 |      0 |      0 |      0 |
   | 29 |      0 |      0 |      0 |      0 |
   | 30 |      0 |      0 |      0 |     0 |
   | 31 |      0 |      0 |      0 |      0 |
