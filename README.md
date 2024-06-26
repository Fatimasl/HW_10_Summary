# 1. Перечень автоматизируемых сценариев

## 1.1. Открыта страница https://netology.ru/
1) На странице в части "Направления обучения" нажать на тикет "Программирование";
2) система откроет https://netology.ru/development

ИЛИ

1) Нажать на кнопку "Каталог курсов";
2) система откроет всплывающее меню, в котором нажать на овальную кнопку "Программирование";
3) система откроет https://netology.ru/development

ИЛИ

1) Нажать на кнопку "Каталог курсов";
2) система откроет всплывающее меню, в котором нажать на овальную кнопку "Все курсы";
3) система откроет https://netology.ru/navigation
4) нажать на овальную кнопку "Программирование";
5) система откроет https://netology.ru/development

ИЛИ

1) Нажать на кнопку "Каталог курсов";
2) система откроет всплывающее меню, в котором нажать на овальную кнопку "Все курсы";
3) система откроет https://netology.ru/navigation

## 1.2. Открыта страница https://netology.ru/development или https://netology.ru/navigation:
### 1.2.1. Успешный кейс перехода на страницу с профессией
1) пролистать перечень профессий и найти на странице профессию "Инженер по тестированию";
2) нажать на надпись "Инженер по тестированию";
3) система откроет страницу с профессией https://netology.ru/programs/qa

### 1.2.2. Успешный кейс перехода на страницу с профессией
1) установить фильтр "Платное" в группе фильтров "Стоимость";
2) система откроет перечень отфильтрованных профессий;
2) пролистать перечень и найти на странице профессию "Инженер по тестированию";
3) нажать на надпись "Инженер по тестированию";
4) система откроет страницу с профессией https://netology.ru/programs/qa

### 1.2.3. Успешный кейс проверки отсутствия возможности перехода на страницу с профессией
1) установить только фильтр "Бесплатное" в группе фильтров "Стоимость";
2) система откроет перечень отфильтрованных профессий;
3) Пролистать перечень, убедиться, что профессия "Инженер по тестированию" отсутствует;

### 1.2.4. Успешные кейсы перехода на страницу с профессией и проверки отсутствия возможности перехода на страницу с профессией
1) аналогичным образом, как это указано в 1.2.2-1.2.3 установить по отдельности каждый возможный фильтр из каждой группы фильтров (из следующих групп: "С документами", "Длительность", "Уровень", "Навыки"). Пролистать перечень отфильтрованных профессий, убедиться, что профессия "Инженер по тестированию" присутствует и перейти в нее, либо отсутствует (итого максимум 40 тестов на странице https://netology.ru/development и 116 тестов на странице https://netology.ru/navigation). Тестировать отбор отфильтрованных профессий по совокупности одновременно установленных фильтров из различных групп фильтров нужно только в том случае, если позволяет бюджет и сроки тестирования, уже после окончания всего остального функционального тестирования;

### 1.2.5. Успешный кейс перехода на страницу с профессией
1) в поисковой строке написать строку поиска "тестирование", а затем нажать кнопку "Найти курс";
2) система откроет перечень отфильтрованных профессий;
3) пролистать перечень и найти на странице профессию "Инженер по тестированию";
4) нажать на надпись "Инженер по тестированию";
5) система откроет страницу с профессией https://netology.ru/programs/qa

### 1.2.6. Успешный кейс перехода на страницу с профессией
1) в поисковой строке написать строку поиска "тестирование";
2) система во всплывающей подсказке покажет подходящие курсы;
3) выбрать и нажать на "Инженер по тестированию";
4) система откроет страницу с профессией https://netology.ru/programs/qa

### 1.2.7. Успешный кейс перехода на страницу с профессией
1) пролистать перечень профессий, найти профессию "Инженер по тестированию" и нажать напротив нее "сердечко";
2) затем нажать на "Избранное" (над группа фильтров);
3) система откроет страницу https://netology.ru/favorites;
4) пролистать перечень избранного, найти профессию "Инженер по тестированию";
5) нажать на надпись "Инженер по тестированию";
6) система откроет страницу с профессией https://netology.ru/programs/qa

## 1.3. Открыта страница с профессией https://netology.ru/programs/qa (под неавторизованным пользователем)
1) нажать кнопку "Записаться" в верхней части страницы;
2) система промотает страницу до конца до формы "Запишитесь на курс";
- либо самостоятельно промотать страницу до конца до формы "Запишитесь на курс";

Далее описаны шаги взаимодействия с формой "Запишитесь на курс" на странице профессии.

### 1.3.1. Успешный кейс записи на курс
3) ввести в поле Имя сгенерированное на кириллице Имя;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) ввести в поле Электронная почта сгенерированный емейл;
6) нажать Записаться;
7) система сообщит об успешной записи на курс и отправит на страницу авторизации.

### 1.3.2. Неуспешный кейс записи на курс (пустое имя)
3) очистить поле Имя;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) ввести в поле Электронная почта сгенерированный емейл;
6) нажать Записаться;
7) система сообщит об ошибке под полем Имя "Обязательное поле".

### 1.3.3. Неуспешный кейс записи на курс (пустой телефон)
3) ввести в поле Имя сгенерированное на кириллице Имя;
4) очистить поле Телефон;
5) ввести в поле Электронная почта cгенерированный емейл;
6) нажать Записаться;
7) система сообщит об ошибке под полем Телефон "Обязательное поле".

### 1.3.4. Неуспешный кейс записи на курс (пустой емейл)
3) ввести в поле Имя сгенерированное на кириллице Имя;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) очистить поле Электронная почта;
6) нажать Записаться;
7) система сообщит об ошибке под полем Электронная почта "Обязательное поле".

### 1.3.5. Неуспешный кейс записи на курс (Имя со спец.символами)
3) ввести в поле Имя сгенерированное на кириллице Имя и добавить один из спец символов !"№;%:?*()+@#$^&;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) ввести в поле Электронная почта сгенерированный емейл;
6) нажать Записаться;
7) система сообщит об ошибке под полем Имя "Должно состоять из букв".

### 1.3.6. Неуспешный кейс записи на курс (Телефон из 6 цифр)
3) ввести в поле Имя сгенерированное на кириллице Имя;
4) ввести в поле Телефон сгенерированный телефон (как + и далее 6 цифр);
5) ввести в поле Электронная почта cгенерированный емейл;
6) нажать Записаться;
7) система сообщит об ошибке под полем Телефон "Должно состоять минимум из 11 цифр".

### 1.3.7. Неуспешный кейс записи на курс (емейл без @)
3) ввести в поле Имя сгенерированное на кириллице Имя;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) ввести в поле Электронная почта cгенерированный емейл, но убрать из него символ @;
6) нажать Записаться;
7) система сообщит об ошибке под полем Электронная почта "Ошибка ввода".

### 1.3.8. Неуспешный кейс записи на курс (емейл без домена)
3) ввести в поле Имя сгенерированное на кириллице Имя;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) ввести в поле Электронная почта cгенерированный емейл, но убрать из него все символы после @;
6) нажать Записаться;
7) система сообщит об ошибке под полем Электронная почта "Ошибка ввода".

### 1.3.9. Неуспешный кейс записи на курс (емейл без точки)
3) ввести в поле Имя сгенерированное на кириллице Имя;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) ввести в поле Электронная почта cгенерированный емейл, но убрать из него символ ".";
6) нажать Записаться;
7) система сообщит об ошибке под полем Электронная почта "Ошибка ввода".

### 1.3.9. Неуспешный кейс записи на курс (емейл без логина)
3) ввести в поле Имя сгенерированное на кириллице Имя;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) ввести в поле Электронная почта cгенерированный емейл, но убрать из него все символы до @;
6) нажать Записаться;
7) система сообщит об ошибке под полем Электронная почта "Ошибка ввода".

### 1.3.10. Неуспешный кейс записи на курс (Имя из одного символа)
3) ввести в поле Имя один символ на кириллице;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) ввести в поле Электронная почта сгенерированный емейл;
6) нажать Записаться;
7) система сообщит об ошибке под полем Имя "Должно быть не короче 2 символов".

### 1.3.11. Успешный кейс записи на курс (Имя из двух символов)
3) ввести в поле Имя два символа на кириллице;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) ввести в поле Электронная почта сгенерированный емейл;
6) нажать Записаться;
7) система сообщит об успешной записи на курс и отправит на страницу авторизации.

### 1.3.12. Успешный кейс записи на курс (Имя из трех символов)
3) ввести в поле Имя два символа на кириллице и дефис;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) ввести в поле Электронная почта сгенерированный емейл;
6) нажать Записаться;
7) система сообщит об успешной записи на курс и отправит на страницу авторизации.

## 1.4. Открыта страница с профессией https://netology.ru/programs/qa (под неавторизованным пользователем)
0) авторизоваться на сайте;
1) нажать кнопку "Записаться" в верхней части страницы;
2) система промотает страницу до конца до формы "Запишитесь на курс". Система в форме "Запишитесь на курс" предзаполнила Имя и Телефон из данных пользователя, указанных в личном кабинете;

- либо самостоятельно промотать страницу до конца до формы "Запишитесь на курс";

Далее описаны шаги взаимодействия с формой "Запишитесь на курс" на странице профессии.

### 1.4.1. Успешный кейс записи на курс (пользователь еще не был записан на курс)
3) нажать Записаться;
4) система сообщит об успешной записи на курс и отправит на страницу оплаты курса.

### 1.4.2. Успешный кейс записи на курс (пользователь уже был записан на курс, но не оплатил его)
3) нажать Записаться;
4) система сообщит об успешной записи на курс и отправит на страницу оплаты курса;
5) открыть страницу с профессией https://netology.ru/programs/qa
6) нажать Записаться в форме "Запишитесь на курс"
7) система сообщит об успешной записи на курс и отправит на страницу оплаты курса.

### 1.4.3. Успешный кейс записи на курс (пользователь уже оплатил данный курс)
3) нажать Записаться;
4) система сообщит об успешной записи на курс и отправит на страницу оплаты курса;
5) произвести оплату курса;
6) система сообщит об успешной оплате курса и отправит на страницу "Моё обучение";
7) открыть страницу с профессией https://netology.ru/programs/qa
8) нажать Записаться в форме "Запишитесь на курс"
9) система сообщит об успешной записи на курс и отправит на страницу "Моё обучение".

### 1.4.4. Успешный кейс записи на курс (авторизованный пользователь записывается на курс, указывая другие Имя и Телефон)
3) ввести в поле Имя сгенерированное на кириллице Имя;
4) ввести в поле Телефон сгенерированный телефон (как +7 и далее 10 цифр);
5) нажать Записаться;
6) система сообщит об успешной записи на курс и отправит на страницу авторизации под новыми значениями полей Имя и Телефон.

# 2. Перечень используемых инструментов с обоснованием выбора

## 2.1. Page Object
Данный инструмент должен использоваться, потому что в тестировании участвует несколько страниц со своей логикой работы, которую можно зашить в отдельные классы, а в тестовых методах только вызывать нужные методы классов Page Object

## 2.2. Подключение к базе данных
База данных нужна для хранения регистрационных данных зарегистрированных пользователей, чтобы проверить те сценарии, которые запускаются под авторизованным пользователем. Регистрация пользователей не входит в тестируемые сценарии, поэтому пользователи должны быть зарегистрированы заранее. Их должно быть несколько, т.к. почти каждый из тестов заканчивается записью на курс, а значит следующий тест мы должны производить уже под другим пользователем, который еще не записан на курс.

## 2.3. Репортинг Allure
Удобный репортинг для наглядного получения результатов тестирования

## 2.4. Faker
Инструмент для генерации имен, телефонов и email

# 3. Перечень необходимых разрешений, данных и доступов

- jar-файл с SUT, при запуске которого создаются 10 авторизованных пользователей, регистрационные данные которых складываются в базу данных;
- доступ к API SUT и описание метода регистрации пользователя (для возможности самостоятельно создать  авторизованных пользователей в случае, если при запуске jar-файла авторизованные пользователи не создаются);
- доступ к API SUT и описание метода изменения статуса оплаты курса "Инженер по тестированию" для зарегистрированного пользователя;
- доступы подключения к базе данных с уже существующими авторизованными пользователями, учетные записи которых можно использовать для тестирования (тип СУБД, url, login, password);
- адрес проекта на github или доступ к системе управления проектами, которая используется в команде разработки и в которой можно было бы зафиксировать issue-отчет об ошибке. 

# 4. Перечень и описание возможных рисков при автоматизации

- отсутствие тестовых ID у элементов на страницах, отсутствие возможности добавить тестовые ID. Привязка выбора проверяемых элементов в автотестах к элементам страницы, которые могут измениться (они могут изменить своё расположение на странице, могут быть удалены, переименованы), в результате автотесты перестанут работать.

# 5. Перечень необходимых специалистов для автоматизации

- автотестировщик

# 6. Интервальная оценка с учётом рисков в часах
- создание класса тестовых данных "DataHelper" (2-3 часа)
- создание классов работы со страницами (Page Object) (24-32 часа)
- создание класса работы с базой данных авторизованных пользователей "SQLHelper" (2-4 часа)
- наполнение базы данных авторизованными пользователями (2-4 часа)
- автотесты по сценариям 1.1 (1-2 часа)
- автотесты по сценариям 1.2 без 1.2.4 (1-2 часа)
- автотесты по сценариям 1.3 (2-3 часа)
- автотесты по сценариям 1.4 (2-3 часа)
- подключение allure - (1 час)
- автотесты по сценариям 1.2.4 (4-5 часов)
- страховой запас на риски 16 часов

ИТОГО 57 - 75 часов