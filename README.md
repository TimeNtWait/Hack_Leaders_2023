### Хакатон "Лидеры цифровой трансформации" 2023
#### Задача №5 
Разработать ML–модель, которая по названиям, атрибутам и картинкам сможет ответить на вопрос являются ли
два товара одинаковыми.

Реализованное решение включает в себя:
- формирвоание новых многообразных признаков.
- реализация признака определяющего важность аттрибутов товаров
- борьба с дисбалансами классов: Over и Under сэмплирование, TomekLinks, взвешивание классов, генерация новых данных используюя сущесвтующие
- использование N-грамм
- ансамблирование по доменам  

#### Архитектура решения:
Ансамблирование по доменам данных, для каждой группы товаров обучалась своя модель, т.к. важность определенных признаков для каждого типа товара различные. Внутри каждой группы использовался собственный ансамбль из CatBoost, BalancedBagging и LightGBM. Итоговый стекинг решения производился через голосование.  


![](docs/image.png)

#### Докментация (docs/):
- Презентация
- Подробная документация
- Сводка экспериментов с метриками и описанием
- Описание Фичей
- План работ

https://miro.com/app/board/uXjVMIsTp2E=/
