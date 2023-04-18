# Курс по изучению Java. Часть 1.

## Результат: серверное приложение, предоставляющее API для взаимодействия с любым приложением-клиентом.

### Приобретенные навыки: 

- java-core;
- unit-тестирование;
- postgresql;
- docker и deploy(публикация) образа приложения на docker-hub;
- понимание ООП-парадигмы в программировании;
- понимание и применение принципов SOLID;
- базовые знания архитектурных и дизайн паттернов проектирования приложений;
- java reflection-api;
- web-socket;
- базовые знания о работе со сборщиками проектов и зависимостями;
- создание собственной библиотеки и ее расположение в общедоступном репозитории (создание артефакта);
- подключение библиотеки к проекту; 
- работа в команде по ТЗ;
- deploy(публикация) проекта в сети интернет.

# ТЕХНИЧЕСКОЕ ЗАДАНИЕ:

### Создать серверное приложение калькулятор, принимающее на вход математическое выражение любого вида, т.е:

1. Разрешены скобки ();
2. Разрешен унарный минус -5 + 7;
3. Изначально поддерживаются операторы +, -, *, /, =;

### ... и вычисляющее значение выражения любой сложности. Все выражения с ответами, которые присылают пользователи,
###должны быть сохранены в базу данных в формате: число, время, выражение, ответ 

## Особые условия: 
1. Придерживаться парадигмы ООП и принципов SOLID;

> Например, при добавлении в приложение нового оператора(допустим, извлечение корня) 
> код должен измениться лишь в одном месте приложения.

###### Ссылка на подобное приложение: <http://blckrbbit.ru:8008/>

# Порядок выполнения.

> Работа над задачей разбита на "спринты", спринты содержат теоретическую и практическую части.
> Каждый спринт сопровождается код-ревью.
> Переход к следующему спринту возможен только после approve кода практической части.
> Каждый спринт выполняется в отдельной ветке, отходящей от ветки dev
> Ветка спринта сливается с веткой dev после approve
> Ветка dev сливается с основной веткой после полной готовности приложения

## СПРИНТ № 1.

### Теория.

###### 1. Что такое класс в java? 
> Ссылки:
- <https://javarush.com/groups/posts/1949-znakomstvo-s-klassami-napisanie-sobstvennihkh-klassov-konstruktorih>
- <https://www.youtube.com/watch?v=uPK2FVz6qUs>

###### 2. Что такое интерфейс в java?
> Ссылки: 
- <https://javarush.com/groups/posts/1981-dlja-chego-v-java-nuzhnih-interfeysih>
- <https://www.youtube.com/watch?v=uCgF5-yCbGA&t=5s>

###### 3. Java класс Object.
> Ссылки:
- <https://metanit.com/java/tutorial/3.9.php>
- <https://www.youtube.com/watch?v=KEQ043yT3F4>

###### 4. Java интерфейс Collection.
> Ссылки:
- <https://www.examclouds.com/ru/java/java-core-russian/interface-collection> (тут же ссылки на описание других коллекций в java)
- <https://proglang.su/java/collections>
- <https://www.youtube.com/watch?v=RBDXuOMlvxk&list=PL8X2nqRlWfab2fMfRCADxQfUUPyaAe842> ссылка на playlist обо всех коллекциях
- <https://www.youtube.com/watch?v=-S_huEuNJiU&list=RDCMUCdXqgQdGW5go6nkkBbUVSMA&index=1> отличный курс по коллекциям, стоит посмотреть весь

###### 5. Java интерфейс List и его реализация ArrayList.
> Ссылки:
- <https://javarush.com/groups/posts/klass-arraylist>
- <https://www.youtube.com/watch?v=QCjLMw988kQ&t=10s>

###### 6. Java интерфейс Map и его реализация HashMap.
> Ссылки:
- <https://javarush.com/groups/posts/1940-klass-hashmap- >
- <https://www.youtube.com/watch?v=DpHI6yRT6Es>
- <https://www.youtube.com/watch?v=BYJHHJplDRA>

###### 7. Java методы equals() и hashCode().
> Ссылки:
- <https://www.youtube.com/watch?v=ZcZQEqxmjOQ> 
- <https://javarush.com/groups/posts/2179-metodih-equals--hashcode-praktika-ispoljhzovanija>

###### 8. Java интерфейс Set и его реализация HashSet.
- <https://javarush.com/groups/posts/2147-hashset-v-java>
- <https://www.youtube.com/watch?v=-S_huEuNJiU&t=1s>
- 
###### 9. Java класс Stack.
> Ссылки:
- <https://javarush.com/groups/posts/2321-strukturih-dannihkh--stek-i-ocheredjh>
- <https://www.youtube.com/watch?v=JKv-vCjJTVA>

###### 10. Обратная польская постфиксная запись математических выражений.
> Ссылки:
- <http://aliev.me/runestone/BasicDS/InfixPrefixandPostfixExpressions.html>
- <https://www.youtube.com/watch?v=sC566vzV9B0&t=455s>

### Практика.

1. Написать алгоритм перевода инфиксной нотации (например, 2 + 2) в постфиксную(22+);
2. Написать алгоритм вычисления постфиксного выражения;

> Ссылка на разбор логики такого калькулятора: <https://www.youtube.com/watch?v=Vk-tGND2bfc>
> Ссылка на туториал на youtube c примером кода: <https://www.youtube.com/watch?v=6AMp0zH7x7M&t=2s>

## Примечание: перед код-ревью запланируем встречу, где обговорим все, что осталось непонятным, я отслежу прогресс.

## СПРИНТ № 2.

### Теория.

### Практика.