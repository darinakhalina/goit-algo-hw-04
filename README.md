# Висновки.

## Тестові данні:
Були використані для тестування малі данні (100 елементів), середні данні (1,000 елементів) та великі данні (10,000 елементів).

| Алгоритм             | Час для малих даних  | Час для середніх даних | Час для великих даних |
| :------------------- | :------------------- | :--------------------- | :-------------------- |
| Сортування sort      | 0.00005              | 0.00060                | 0.01044               |
| Сортування sorted    | 0.00005              | 0.00064                | 0.01057               |
| Злиття merge         | 0.00129              | 0.01399                | 0.18524               | 
| Вставки insertion    | 0.00116              | 0.12556                | 13.49233              |

### Сортування sort та sorted.
Кращий результат. Алгоритми використовують ефективні вбудовані механізми Python для сортування, що робить їх швидкими для всіх обсягів даних. Sort показав себе трохи краще, тому що працює напряму з даними. Sorted - копіює дані. Але в цілому оба ефективні.

### Сортування злиттям (merge).
Повільніший за sort та sorted, використовує додаткову пам'ять для об'єднання.

### Сортування вставками (insertion).
Найповільніший. Його квадратична складність стає помітною для великих даних через необхідність багаторазового перебору та переміщення елементів.
