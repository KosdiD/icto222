# Розумний будинок у довкільній віртуальній та доповненій реальності

Цей проєкт є інтерактивною WebXR симуляцією, що дозволяє користувачам досліджувати віртуальний "розумний будинок", наповнений пристроями Інтернету речей (IoT). Головна мета — продемонструвати концепції IoT, Edge Computing та застосування моделей машинного навчання (ML) безпосередньо на клієнтському пристрої (Edge ML) в імерсивному середовищі.

Користувачі можуть вільно переміщатися по 3D-сцені, взаємодіяти з віртуальними об'єктами, додавати власні IoT-пристрої та керувати ними за допомогою графічного інтерфейсу або голосових команд.

## 🎯 Мета проєкту: Інтернет речей у доповненій реальності

Проєкт візуалізує, як доповнена та віртуальна реальність можуть слугувати інтуїтивним інтерфейсом для керування та моніторингу складної екосистеми IoT, переносячи концепції "туманних" та "периферійних" обчислень у наочний формат.

## 🚀 Функціональність

### 1. Симуляція IoT екосистеми
Користувачі можуть динамічно розміщувати у просторі маркери, що симулюють різноманітні IoT-пристрої. Кожен пристрій має свої унікальні характеристики:
* **Тип пристрою:** Вибір з-поміж стандартних та спеціалізованих ML-пристроїв.
* **Класифікація Edge ML:** Можливість додати пристрої, що симулюють периферійні обчислення, такі як:
    * 👁️ **Computer Vision:** Камери для розпізнавання об'єктів та людей.
    * 🔊 **Аудіо ML:** Процесори для обробки голосових команд та звуків.
    * 📊 **Сенсорна аналітика:** Пристрої для аналізу даних та прогнозування.
    * 🏃 **Детектори руху:** ML-системи для аналізу активності та поведінки.
    * 🌡️ **Клімат ML:** Розумні контролери для оптимізації температури.
    * 💡 **Розумне світло:** Адаптивні системи освітлення.
* **Інформаційна панель:** При кліку на маркер відображається детальна інформація про пристрій, його статус, опис та симульовані ML-моделі.

### 2. Edge Computing та Туманні обчислення
Весь додаток працює у браузері користувача, що є прямою ілюстрацією **Edge Computing**. Всі обчислення, включаючи рендеринг 3D-графіки, логіку симуляції та обробку голосових команд, виконуються на клієнтському пристрої. Це забезпечує низьку затримку та не вимагає постійного з'єднання з потужним сервером.

### 3. ML на периферії (Edge ML)
Ключовою особливістю проєкту є реалізація **голосового керування**, що працює повністю на стороні клієнта.
* **Технологія:** Використовується Web Speech API браузера для розпізнавання мови в реальному часі. Це приклад Edge ML, оскільки аудіопотік обробляється локально.
* **Підтримка української мови:** Система налаштована на розпізнавання команд українською (`lang: 'uk-UA'`).
* **Доступні команди:** Реалізовано широкий спектр команд для керування симуляцією:
    * **Створення об'єктів:** "створити маркер", "створити світло".
    * **Навігація:** "на початок", "додому".
    * **Керування сценою:** "показати/сховати маркери", "експорт".
    * **Керування освітленням:** "увімкнути/вимкнути світло", "яскравість [число]", "зроби світло [колір]" (напр., "зроби світло зелений").

### 4. Додаткові можливості
* **Керування освітленням:** Можливість створювати джерела світла, вмикати/вимикати їх усі разом, регулювати глобальну яскравість та змінювати колір світла за допомогою голосових команд.
* **Кастомізація простору:** Реалізовано функціонал для створення стін, що дозволяє користувачам модифікувати віртуальне середовище.
* **Збереження та завантаження сцени:** Можливість експортувати поточний стан сцени (розміщення маркерів, джерел світла, стін) у файл `.json` та імпортувати його назад.

## 🛠️ Технології та Інструменти

### Використані технології
* **A-Frame (`v1.5.0`):** Основний фреймворк для створення WebXR-додатків.
* **Three.js:** 3D-бібліотека, що лежить в основі A-Frame.
* **TensorFlow.js (`v4.11.0`):** Бібліотека для машинного навчання в браузері.
* **TensorFlow Speech Commands Model (`v0.5.4`):** Спеціалізована модель для розпізнавання голосових команд.
* **Web Speech API:** Нативний API браузера для реалізації голосового керування.
* **HTML5, CSS3, JavaScript (ES6+):** Стандартні веб-технології для побудови інтерфейсу та логіки додатку.

### Залучені AI-моделі
Для генерації та структурування документації, а також для аналізу коду, були використані наступні моделі штучного інтелекту:
* Платна версія Gemini 2.5 PRO
* Платна версія Claude Opus 4
* Безкоштовна версія ChatGPT
* Безкоштовна версія DeepSeek
