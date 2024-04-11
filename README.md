# -SQL_Test_Task-
# Тестовое задание №1

## Таблица Meals
| MealID | MealName   | Price | DrinkID |
|--------|------------|-------|---------|
| 1      | Omlet      | 120   | 1       |
| 2      | Fried Egg  | 70    | 4       |
| 3      | Sausage    | 90    | 3       |

## Таблица Drinks
| DrinkID | DrinkName    |
|---------|--------------|
| 1       | Orange Juice |
| 2       | Tea          |
| 3       | Cofee        |
| 4       | Milkshake    |

Напишите запрос, который выведет всю информацию по завтракам и напиткам, которые прилагаются к завтраку с условием, что цена завтрака должна быть не менее 90.

### Описание полей:
- MealID – первичный ключ для таблицы Meals. Присваивает уникальный номер для каждого продукта
- MealName - наименование продукта
- Price – цена
- DrinkID – первичный ключ для таблицы Drinks (и внешний для таблицы Meals)
______________________________________________________________________________________________________________________________
- # Тестовое задание №2

В базе данных есть 2 таблицы.

Первая содержит информацию о том, из какого города (Start) в какой (End) вылетает самолет, и есть ли на самолет билеты в продаже (Tickets). Вторая содержит длительность соответствующего перелета в минутах Duration_min.

Необходимо написать SQL запрос, который будет искать рейсы из Екатеринбурга с билетами в наличии и длительностью полета не более (или равно) 3 часов, результаты должны быть отсортированы по возрастанию длительности полета.

## Table 1. Flights
| Id | Start            | End          | Tickets |
|----|------------------|--------------|---------|
| 1  | Ekaterinburg     | Moscow       | true    |
| 2  | Saint-Petersburg | Ekaterinburg | false   |
| 3  | Vladivostok      | Kaliningrad  | true    |
| 4  | Ekaterinburg     | Moscow       | true    |
| 5  | Ekaterinburg     | Saint-Petersburg | false |
| 6  | Samara           | Moscow       | true    |
| 7  | Ekaterinburg     | Kaliningrad  | false   |
| 8  | Moscow           | Ekaterinburg | true    |
| 9  | Samara           | Saint-Petersburg | false |
| 10 | Ekaterinburg     | Vladivostok  | true    |

## Table 2. Duration
| Id | Duration_min |
|----|--------------|
| 1  | 120          |
| 2  | 150          |
| 3  | 540          |
| 4  | 125          |
| 5  | 150          |
| 6  | 100          |
| 7  | 180          |
| 8  | 120          |
| 9  | 110          |
| 10 | 480          |


