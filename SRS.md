
____

## **Оглавление**

- [1. Введение](#intro)
- [2. Требования пользователя](#user_requirements)
  - [2.1 Программные интерфейсы](#interfaces)
  - [2.2 Интерфейс пользователя](#ui)
  - [2.3 Характеристики пользователей](#user_characteristics)
  - [2.4 Предположения и зависимости](#assumptions)
- [3. Системные требования](#system_requirements)
  - [3.1 Функциональные требования](#functional_requirements)
  - [3.2 Нефункциональные требования](#non_functional_requirements)

<a name="intro"></a>
## **1. Введение**

**Название проекта:** lines

**Технологии и инструменты разработки:**

•	Язык разработки: Kotlin.

•	Фреймворк для создания UI: XML.

•	Среда разработки: Android Studio.

**Описание проекта:**  
Проект представляет собой мобильное приложение для бронирования авиабилетов. Пользователи могут искать интересующие рейсы или выбирать из предложенного списка рейсов.

**Границы проекта:**  
Приложение не предоставляет функций отслеживания самолётов, а так же других авиа-услуг.

<a name="user_requirements"></a>
## **2. Требования пользователя**

<a name="interfaces"></a>
### **2.1 Программные интерфейсы:**

Продукт будет взаимодействовать с несколькими внешними системами:

• Firebase Authentication для авторизации и хранения данных пользователей.

• Transaction Database для локального хранения информации о различных рейсах.

<a name="ui"></a>
### **2.2 Интерфейс пользователя:**

Приложение будет содержать следующие основные интерфейсы:

• Окно загрузки приложения.
  
  ![Окно загрузки приложения](https://github.com/maxon230501/lab2_jcrpo/blob/main/mockups/loading_screen.png)


• Окно регистрации нового пользователя.
  
  ![Окно регистрации нового пользователя](https://github.com/maxon230501/lab2_jcrpo/blob/main/mockups/regisrate_screen.png)

• Окно входа для зарегистрированного пользователя.
  
  ![Окно входа для зарегистрированного пользователя](https://github.com/maxon230501/lab2_jcrpo/blob/main/mockups/first_screen.png)



• Окно для просмотра карты места вылета.
  
  ![Окно для просмотра карты места вылета](https://github.com/maxon230501/lab2_jcrpo/blob/main/mockups/map_screen.png)

• Окно для поиска рейса.
  
  ![Окно для поиска рейса](https://github.com/maxon230501/lab2_jcrpo/blob/main/mockups/search_screen.png)

• Окно для просмотра популярных авиабилетов.
  
  ![Окно для просмотрапопулярных авиабилетов](https://github.com/maxon230501/lab2_jcrpo/blob/main/mockups/flight_screen.png)

  Пример взаимодействия:

| Действие пользователя                          | Реакция системы                                               |
|------------------------------------------------|---------------------------------------------------------------|
| Нажимает "Вход" в стартовом окне               | Проверка данных и вход в систему                              |
| Нажимает на икону рейса                        | Открывается окно для добавления брони и просмотра информации  |
| Нажимает на иконку поиска                      |Открывается окно для поиска рейса                              |
| Нажимает на иконку карты                       | Открывается окно для просмотра карты места вылета             |

<a name="user_characteristics"></a>
### **2.3 Характеристики пользователей:**

•	Пользователи страше 18 лет: Люди имеющие свой доход и запланированные траты, которым необходимо совершать авиа перелёты.


<a name="assumptions"></a>
### **2.4 Предположения и зависимости:**

•	Все пользователи должны иметь подключение к интернету для синхронизации данных с облаком.

•	Приложение будет работать только на устройствах с Android 5.0 и выше.

<a name="system_requirements"></a>
## **3. Системные требования**

<a name="functional_requirements"></a>
### **3.1 Функциональные требования:**

• Приложение должно позволять пользователям добавлять, просматривать рейсы.

• Приложение должно правильно и интуитивно понятно показывать карты для простого восприятия места посадки.

• Авторизация должна быть обязательной для сохранности личных данных пользователей.

• Приложение должно поддерживать синхронизацию данных с облаком (Firebase).

<a name="non_functional_requirements"></a>
### **3.2 Нефункциональные требования:**

•	Безопасность: Данные пользователей должны быть защищены, а авторизация — проводиться через надёжную систему (например, Firebase Authentication).

•	Производительность: Приложение должно загружаться и работать плавно на большинстве современных устройств.

•	Удобство использования: Интерфейс должен быть интуитивно понятным, особенно для пользователей с базовыми техническими навыками.
