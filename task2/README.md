
## Алгоритмы и структуры данных: Задача 2, ход коня.

### Постановка задачи

```
  С помощью известного алгоритма выяснить максимальное количество возможных
  ходов коня на доске. Возможно ли обойти доску полностью.
```

Входные данные:
```
  На вход подаются координаты двух заблокированых ячеек и координаты коня на сетке.
```

Условия выполнения:
```
– Сетка 7х9,
– Две клетки заблокированы (для ходов)
– Вывести 2 результата работы программы: успешный полный обход, неуспешный обход.
– Вывести результат на экран символьной графикой (пошагово).
```

Входные данные для проверки:
```
  (1) Координаты заблокированных клеток: (1,1), (2,2).
    Старт фигуры с координат: (1,3) - не полный обход
    Старт фигуры с координат: (1,2) - полный обход
```

### header file (используемые функции)

```cpp

// Печатает сетку со всеми (пройденными) ходами коня, заблокированными клетками
void printHorse(int position[ROWS][COLUMNS], int ROWS, int COLUMNS);
// Задает координаты для x, y
void setCoordinates(int &x, int &y);

// Определяет является ли координата (x, y) внутри доски
int isInsideBoard(int x, int y);
// Спрашивает пользователя какое количество заблокированных клеток создать
int getBlockedCellsAmount();

```
