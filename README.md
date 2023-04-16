# Алгоритмы и структуры данных (ADS-7)

![GitHub pull requests](https://img.shields.io/github/issues-pr/NNTU-CS/ADS-7)
![GitHub closed pull requests](https://img.shields.io/github/issues-pr-closed/NNTU-CS/ADS-7)

Срок выполнения задания:

**до 30.04 ** 

![Relative date](https://img.shields.io/date/1682888400)

## Задание

> Написать реализацию структуры данных "очередь с приоритетом" **TPQueue** на связанном списке

## Пояснение

В данной задаче необходимо написать реализацию разновидности очереди - **Очередь с приоритетами**, работа которой строится по следующей схеме:

Очередь обрабатывает символы, каждому из которых назначается *приоритет*, - целое число от 1 до 10. При поступлении в очередь элементов, они занимают места, в соответствии с приоритетом: чем он больше, тем ближе к началу очереди. При получении элемента из очереди, вперед идут элементы, чей приоритет больше.

Вставка элемента в очередь должна иметь вычислительную сложность O(n), выборка элемента из очереди, - O(1).

В качестве типа данных **T**, используемого очередью, возьмем структуру *SYM*:

```c++
struct SYM {
  char ch;
  int prior;
};
```
## Программная реализация

Очередь должна строиться как связанный список, при добавлении элементов, они вставляются в нужную позицию, при извлечении, - они удаляются из головы.

Сам список может быть односвязным или двусвязным.


## Выполнение работы

- Предполагается, что тип **T** внутри очереди будет структурой, состоящей из двух полей, приоритет задается полем **prior**.
- Поместить описание шаблона **TPQueue** в файл **include/tpqueue.h**
- Изучить файл с тестами **test/tests.cpp** чтобы увидеть примеры использования шаблона очереди с приоритетами.

