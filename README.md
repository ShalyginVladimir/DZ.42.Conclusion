# Домашнее задание к занятию «4.2. Заключительная лекция»

#  Необходимо запланировать тестирование возможности записаться на обучение профессии «Тестировщик ПО»

# План автоматизации тестирования

# 1. Сцинарии в навигации:

Сценарий №1. Зайдите на [веб-сайте Нетологии](https://netology.ru/) на стартовой странице кликните:
Направления обучения "Программирование" - Тестировщик ПО - Записаться - Записаться на курс.

Сценарий №2. Зайдите на [веб-сайте Нетологии](https://netology.ru/) на стартовой странице кликните:
меню "Каталог курсов" - Программирование - Тестировщик ПО - Записаться - Записаться на курс.

Сценарий №3. Зайдите на [веб-сайте Нетологии](https://netology.ru/) на стартовой странице кликните:
меню "Каталог курсов" - строка поиска (Какой курс вам нужен) - набираете наименование профессии "Тестировщик ПО" - 
Найти курс - Тестировщик ПО - Записаться - Записаться на курс.

# 1.1. Заполнение формы заявки валидными значениями (сценарий №1, сценарий №2, сценарий №3)
1.1.1. Строка с именем (ввести имя применяя буквы кириллицы, имя не менее двух букв, разрешено применять тире "-", 
букву "ё" (пример имени - Владимир)).

1.1.2. Строка с номером телефона (необходимо ввести одинадцать цифр мобильного номера, первый знак с цифрой код страны 
(+7), далее десять цифр мобильного номера (пример мобильного номера - "+7 999 123 45 67")).

1.1.3. Строка с адресом электронной почты (необходимо ввести адрес применяя латинские буквы, в адресе обязательно должен 
присутствовать символ "@", обязательно прописан домен ".ru" 
(пример адреса электронной почты - vladimir@mail.ru)).

1.1.4. Кликаем на кнопку "Записаться".

Ожидаемый результат (сообщение о принятии завки "Ваша заявка принята")

# 1.2. Заполнение формы заявки не валидными значениями (сценарий №1, сценарий №2, сценарий №3)
1.1.1. Строка с именем, необходимо ввести не валидное значение (применить знаки и цифры 
(пример имени - Влад12имир).

1.1.2. Строка с номером телефона (необходимо ввести одинадцать цифр мобильного номера, первый знак с цифрой код страны
(+7), далее десять цифр мобильного номера (пример мобильного номера - "+7 999 123 45 67")).

1.1.3. Строка с адресом электронной почты (необходимо ввести адрес применяя латинские буквы, в адресе обязательно должен
присутствовать символ "@", обязательно прописан домен ".ru"
(пример адреса электронной почты - vladimir@mail.ru)).

Ожидаемый результат ("Должно состоять из букв").

# 1.3. Заполнение формы заявки не валидными значениями (сценарий №1, сценарий №2, сценарий №3)
1.1.1. Строка с именем (ввести имя применяя буквы кириллицы, имя не менее двух букв, разрешено применять тире "-",
букву "ё" (пример имени - Владимир)).

1.1.2. Строка с номером телефона, необходимо ввести не валидное значение (необходимо ввести пятнадцать цифр мобильного 
номера (пример мобильного номера - +0 000 000 000 000 00)).

1.1.3. Строка с адресом электронной почты (необходимо ввести адрес применяя латинские буквы, в адресе обязательно должен
присутствовать символ "@", обязательно прописан домен ".ru" 
(пример адреса электронной почты - vladimir@mail.ru)).

Ожидаемый результат ("Номер в формате +9 (999) 999-99-99").

# 1.4. Заполнение формы заявки не валидными значениями (сценарий №1, сценарий №2, сценарий №3)
1.1.1. Строка с именем (ввести имя применяя буквы кириллицы, имя не менее двух букв, разрешено применять тире "-",
букву "ё" (пример имени - Владимир)).

1.1.2. Строка с номером телефона (необходимо ввести одинадцать цифр мобильного номера, первый знак с цифрой код страны
(+7), далее десять цифр мобильного номера (пример мобильного номера - +7 999 123 45 67)).

1.1.3. Строка с адресом электронной почты, необходимо ввести не валидное значение (необходимо ввести адрес применяя 
буквы кириллици (пример адреса электронной почты - владимир@mail.ru)).

Ожидаемый результат ("Неверный email").

# 2. Перечень используемых инструментов:
* Браузер "google" - этот браузер при поиске выдает больше вриантов в сфере IT;
* IntelliJ IDEA Community Edition - приемущество этого языка програмирования описать затрудняюсь, так как опыт работы 
только с ним;
* Gradle - система автоматической сборки, в отличие от Maven, Gradle использует направленный ациклический граф для 
определения порядка выполнения задач, поэтому проект создаем на базе Gradle;
* Lombok – это основанная на аннотациях библиотека Java, позволяющая сократить шаблонный код. В Lombok предлагаются 
различные аннотации, цель которых – заменить ненужный повторяющийся код, писать который утомительно, соответственно 
для удобства в работе пользуемся Lombok;
* Selenide - это фреймворк для написания удобных для чтения и обслуживания автоматизированных тестов на Java. Он 
определяет сжатый свободный API, утверждения на естественном языке и творит чудеса для приложений на основе ajax, 
позволяя нам полностью сосредоточиться на бизнес-логике наших тестов;
* Selenium - это набор программ с открытым исходным кодом, которые применяют для тестирования веб-приложений и 
администрирования сайтов локально и в сети. Программы Selenium позволяют автоматизировать действия браузера, 
соответственно без этого инструмента в автоматизированном тестировании не обойтись. 

# 3. Перечень необходимых разрешений, данных и доступов
3.1. Перед началом тестирования интерфейса необходимо сделать запрос и получить подтверждающее разрешение на проведения 
тестирования.

3.2. Произвести запрос тестовых данных.

# 4. Перечень и описание возможных рисков при автоматизации
* Сбои в работе интернета;
* Перегруженная работа сервиса;
* Отсутствие тестовых меток;
* Частое обновление интерфейсов.

# 5. Перечень необходимых специалистов для автоматизации
5.1. Для выполнения данного задания достаточно одного тестировщика ПО.

# 6. Интервальная оценка с учётом рисков в часах
6.1. Для начинающего тестировщика (например как я), для выполнения качественной работы, ориентировочно потребуется три 
рабочих дня (24 часа).