| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
|  1    |пустое   | пустое   |
|  2    | пустое   | неверное значение   |
|  3    | пустое   | secret_sauce|
|  4    | неверное значение|         неверное значение      |
|  5    | неверное значение         | secret_sauce  |
|  6    | неверное значение |пустое |
|  7    | standard_user |secret_sauce |
|  8    | standard_user | пустое |
|  9    | standard_user | неверное значение |
|  10   | locked_out_user|  пустое  |
|  11   | locked_out_user |неверное значение  |
|  12   |locked_out_user  |secret_sauce  |
|  13    | problem_user |неверное значение |
|  14    | problem_user | secret_sauce |
|  15    |problem_user  | пустое |
|  16   | performance_glitch_user | secret_sauce|
|  17   |performance_glitch_user  | пустое |
|  18   |  performance_glitch_user| неверное значение |

## Тест-кейс №1. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ничего не вводить
- в поле "Password" ничего не вводить
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Usrename is required"

## Тест-кейс №2. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ничего не вводить
- в поле "Password" ввести неверное значение
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Usrename is required"

## Тест-кейс №3. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ничего не вводить
- в поле "Password" ввести secret_sauce
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Usrename is required"

## Тест-кейс №4. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести неверное значение
- в поле "Password" ввести неверное значение
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Usrename is required"

## Тест-кейс №5. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести неверное значение
- в поле "Password" ввести secret_sauce
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Usrename is required"

## Тест-кейс №6. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести неверное значение
- в поле "Password" ничего не вводить
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Usrename is required"

## Тест-кейс №7. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести standard_user
- в поле "Password" ввести secret_sauce
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Вход на сайт

## Тест-кейс №8. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести standard_user
- в поле "Password" ничего не вводить
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Password is required"

## Тест-кейс №9. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести standard_user
- в поле "Password" ввести неверное значение
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Password is required"

## Тест-кейс №10. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести locked_out_user
- в поле "Password" ничего не вводить
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Password is required"

## Тест-кейс №11. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести locked_out_user
- в поле "Password" ввести неверное значение
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Epic sadface: Username and password do not match any user in this service"

## Тест-кейс №12. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести locked_out_user
- в поле "Password" ввести secret_sauce
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Epic sadface: Sorry, this user has been locked out"

## Тест-кейс №13. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести problem_user
- в поле "Password" ввести неверное значение
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Epic sadface: Username and password do not match any user in this service"

## Тест-кейс №14. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести problem_user
- в поле "Password" ввести secret_sauce
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Вход на сайт

## Тест-кейс №15. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести problem_user
- в поле "Password" ничего не вводить
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Password is required"

## Тест-кейс №16. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести performance_glitch_user
- в поле "Password" ввести secret_sauce
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Вход на сайт

## Тест-кейс №17. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести performance_glitch_user
- в поле "Password" ничего не вводить
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Password is required"

## Тест-кейс №18. Проверка авторизации
1. Предусловие
- открыта страница авторизации https://www.saucedemo.com/
2. Шаги
- в поле "Username" ввести performance_glitch_user
- в поле "Password" ввести неверное значение
- нажать на кнопку "Login"
3. Ожидаемый результат 
- Ошибка авторизации "Epic sadface: Username and password do not match any user in this service"


