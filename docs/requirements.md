Неавторизованный пользователь

1. Ознакомиться с информацией о проекте Run IT, ответами на частые вопросы
2. Авторизоваться на Run IT (кнопка Войти / кнопка Регистрация – Войти)
- Электронная почта – Пароль 
- через аккаунт Github
3. Зарегистрироваться на Run IT (кнопка Регистрация / кнопка Вход – Создать аккаунт)
- Электронная почта – Логин – Пароль – Подтвердить пароль 
- через аккаунт Github

Авторизованный пользователь

4. Сменить пароль и логин аккаунта
5. Редактировать / писать код в JavaScript
6. Запустить код на выполнение / проверку
7. Сохранить написанный код / сниппет
8. Поделиться сниппетом с другими пользователями 
9. Получать сниппет от других пользователей 

---
Проверака основного функционала
functional:
  - Кнопка Начать кодить - открывается окно редактора
  - Кнопка Регистрация в верхнем меню открывант форму регистрации
  - Проверка формы регистрации (позитивный. Ivanov25@mail.ru, логин Ivanov25, пароль Ivanov25)
  - Регистрация в форме регистрации - создан аккаунт пользователя с логином Ivanov25
  - Войти с помощью Github в поле регистрации - открытие профиля пользователя 
  - Уже есть аккаунт Войти - открывается форма входа в аккаунт
  - Кнопка Войти в верхнем меню - открылась форма входа в аккаунт 
  - Проверка формы входа (позитивный. Ivanov25@mail.ru, пароль Ivanov25)
  - Войти в поле регистрации - открылся профиль пользователя с логином Ivanov25
  - Войти с помощью Github в поле регистрации - открылся профиль пользователя
  - Нет аккаунта Создать аккаунт - открывается форма регистрации
  - Профиль пользователя, кнопка Редактировать - открылась форма редактирования адреса электронной почты и логина.
  - Изменить логин/адрес - Отправить, изменились данные. Отменить и Крестик(закрыть) - форма редактирования данных почта/логин - закрылась.
  - Профиль пользователя, кнопка Выход - открывается поле редактирования кода
  - Форма Сниппеты, Новый снипет - открылась форма для ввода названия сниппета.
  - Предложенное Имя нового сниппета - сохранить / Изменить и Сохранить. Сниппет с заданным именем появился в поле формы. Отмена / Крестик(закрыть) - закрывает форму.
  - Созданный сниппет в в форме Сниппеты - кнопка Открыть. Открывается окно редактора.
  - Окне редактора написать код JS (позитивный. console.log('Hello, World!');). 
  - Окно редактора, слева написан верный код JS, Запустить - в правом окне результат выполнения кода.
  - Окно редактора, в верный код JS внести изменения, Запустить - в правом окне изменившийся результат.
  - Окно редактора, верный код JS, Поделиться - Открылась Форма Поделиться (Название сниппета, две вкладки Ссылка и код вставки, кнопка Скопировать)
  - Форма Поделиться, Кнопка скопировать ссылку/код. Ctrl+V(вставить) в поле кода - ссылка / код вставлена. Крестик - форма закрылась.

Более глубокое тестирование
functional:
- Создать аккаунт с дублирующими данными (негативный. Ivanov22@mail.ru, Ivanov22, пароль  Ivanov22@mail.ru)
- Негативные сценарии регистрации и входа
- Негативный сценарий написания кода другого языка в окне редактора
- Негативный Окно редактора, НЕверный код JS, Запустить ?
  РАСПИШУ БОЛЕЕ ПОДРОБНО В ТЕСТ-КЕЙСАХ
  
 non-functional:
  - На странице Информация о проекте по ссылкам происходит переход (открывается отдельная вкладка браузера) и открывшаяся информация соответствует теме ссылки. 
  - Все пункты списка FAQ на странице Информации о проекте открываются. 
  - При нажатии на Хекслет Run IT открывается окно редактора / на кнопку О проекте окна редактора - страница Информация о проекте
  - Проверка занесения данных пользвателя в БД 
  - Тестирование в различных браузерах (Yandex, Google, Mazila)
  - Нагрузочное тестирование (стабильная работа длительное время)
  - Стрессвое тестирование (одновременно большое количество работающих)
  - Безопасность сервиса в случае(фишинговая атака, чтобы поделить "вирусами" с другими пользователями)
  - Безопасность хранящихся данных пользователей в БД.
 
implicit:
  - Локализация (если за пределами РФ, перевести названия кнопок), возможно сделать переключатель русский/англ?
  - Забыли пароль/вспомнить пароль
  
Хотелось бы
  - Подвердить регистрацию с электронной почты?
  - Кнопка для возврата в профиль из редактора

Дефект во время тестирования
  - Открыта форма Название сниппета с введенным именем, щелчок вне формы приводит к закрытию без возможности ее найти / вернуть  
  - В какой-то момент,самопроизвольно произошел выход из аккаута, войти повторно не получается????? 


