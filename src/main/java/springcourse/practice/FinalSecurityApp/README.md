# FinalSecurityApp
- **Регистрация пользователей**  
  Новые пользователи могут зарегистрироваться, указав логин, год рождения и пароль. Мы в приложение шифруем (хэшируем) пароль
  и сохраняем пользователя в базе данных.

--------------------------------------------

- **Аутентификация и авторизация**  
  При входе (логине) пользователь проходит аутентификацию, а затем получает доступ к определённым страницам и действиям
  в зависимости от своей роли (ROLE_USER или ROLE_ADMIN).

--------------------------------------------

- **Ролевой доступ**
    - **ADMIN** может заходить на страницу `/admin` и выполнять «админские» операции.
    - **USER** (или ADMIN) может просматривать обычные страницы (например, `/hello`).

--------------------------------------------

- **Валидация данных**  
  Проверяем корректность введённых данных при регистрации (например, что логин не занят другим пользователем).