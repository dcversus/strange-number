## Advent of Code — Проверка допустимых игр с кубиками

У тебя есть список строк, каждая из которых описывает некую игру. Каждая строка начинается с номера игры и двоеточия, далее следует одно или несколько «раундов», разделённых точкой с запятой (`;`). В каждом раунде указано, сколько кубиков определённого цвета (красного, зелёного или синего) было вытянуто.

### Пример строки:

Game 3: 3 red, 5 green, 6 blue; 2 red, 1 green

### Условия:
- В одном раунде не должно быть более:
  - **12** красных кубиков
  - **13** зелёных кубиков
  - **14** синих кубиков
- Если **в любом раунде** игры хотя бы один цвет превышает лимит — игра считается **недопустимой**.

### Задача:
1. Разобрать входной текст.
2. Проверить каждую игру на соответствие лимитам.
3. Сложить номера **только допустимых** игр.
4. Странным числом является итоговая сумма.

### Входные данные:

Game 2: 15 red, 1 green
Game 3: 3 red, 5 green, 6 blue
Game 5: 10 red, 2 green, 14 blue
Game 6: 3 red, 14 green
Game 8: 4 red, 3 green, 10 blue
Game 10: 2 red, 3 green, 15 blue
Game 21: 1 red, 1 green, 1 blue