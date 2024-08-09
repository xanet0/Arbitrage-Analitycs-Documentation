<h1>Гайд з налаштування та використання бота</h1>
<details>
  <summary><strong>!!! Правила використання бота !!!</strong></summary>
  
  1. Ні в якому випадку не можна змінювати порядок таблиць в Google Sheets
  2. Не переставляти/додавати колонки в сторінках
  3. Якщо вам просто треба додати апку в табличку і ви не намагались додати самі апку в бота, то писати/телефонувати мені не треба
  4. Звоніть якщо виникли проблеми з ботом
  
</details>
<details>
  <summary>Таблиця не заповнилась</summary>
  
  1. Відкриваємо репозиторій з нашим ботом
  2. Тикаємо зверху на <strong>Actions</strong><br>
  <img src="https://raw.githubusercontent.com/xanet0/Arbitrage-Analitycs-Documentation/main/image/Screenshot_2.png" alt="Фото" style="width: 80%;"><br>
  3. 1. Тикаємо на <strong>Google Sheets API parser</strong>
     2. Жмемо <strong>Run workflow</strong>
     3. Записуємо дату, яку в таблиці нам потрібно оновити<pre><strong>Формат Запису</strong><br>Дата.Місяць.Рік<br>Приклад: 09.04.2024</pre>
     4. Далі тиснемо на <strong>Run workflow</strong> знову
  <img src="https://raw.githubusercontent.com/xanet0/Arbitrage-Analitycs-Documentation/main/image/image_2024-08-09_15-46-09.png" alt="Фото" style="width: 80%;">
</details>
<details>
  <summary>Як заповнити таблицю за інший день</summary><br>
  <strong>В пункті таблиця не заповнилась все розписано</strong><br>
</details>


<details>
  <summary>Додавання нової апки в табличку</summary>
  <h3>Налаштування:</h3>
  
  1. Відкриваємо наш репозиторій та потрібну нам папку
  2. Відкриваємо data.json
  3. В табличці створюємо новий лист з кампаніями
  4. Колонки з сервісами повинні бути обов'язково в такому ж порядку як на інших листах 

  <details>
    <summary><strong>Обов'язкові правила при налаштуванні</strong></summary><br>
    
  При додаванні кампанії або апки в data.json <strong>дуже важливий порядок</strong><br>
  Як потрібно додавати кампанію/апку
    
    Наприклад:
        У нас в табличці такий порядок: Gta USSR, GTA Brazil, Gta Mexico
        Ми хочемо додати GTA Brazil в парсер, в data.json повино вийти так:
        "Gta USSR":"fj438djsdkjf2",
        "Gta brazil":"sdlfsu39d",
        "Gta Mexico":"kdsfhs892df"

  <strong>Примітка</strong>

    Якщо ви додаєте апку в табличку, в самий кінець списку, то при додаванні строки в data.json кома в кінці не повинна стояти "Назву апки":"Campaign Set ID"
    Якщо додаєте апку не в кінці списку, то кома повинна ОБОВ'ЯЗКОВО стояти "Назву апки":"Campaign Set ID",
    
  </details>
  <details>
    <summary><strong>Unity Ads</strong></summary><br>
    <strong>Копіювання Campaign Set ID</strong>
      
    1. Відкриваємо Unity Cloud, User Acquisition
    2. Наводимо курсором на потрібну нам апку
    3. Копіюємо Campaign Set ID:
      
  <img src="https://github.com/xanet0/Arbitrage-Analitycs-Documentation/blob/main/image/Screenshot_4.png" alt="Фото" style="width: 80%;"><br>
  
  
  <strong>Додавання Кампанії в Бота</strong>
  
      
    1. Заходимо в data.json, шукаємо розділ unityAds
    2. Далі орієнтуємося по назвам апок і додаємо нову строку, в тому ж порядку як в табличці
    3. В строці пишемо "Назву апки(можна вказати любу назву)":"Campaign Set ID",
        
  </details>
  
  <details>
    <summary><strong>Unity Monet</strong></summary>><br>
    <strong>Копіювання Android Game ID</strong>
    
    1. Відкриваємо Unity Cloud, Ads Monetization
    2. Вибираємо потрібну нам апку
    3. Жмемо на Ad units
    4. Копіюємо Android Game Id:
    
  <img src="https://github.com/xanet0/Arbitrage-Analitycs-Documentation/blob/main/image/Screenshot_3.png" alt="Фото" style="width: 80%;"><br>

  
  <strong>Додавання Кампанії в Бота</strong>
  
    1. Заходимо в data.json, шукаємо розділ unityMonet
    2. Далі орієнтуємося по назвам апок і додаємо нову строку, в тому ж порядку як в табличці
    3. В строці пишемо "Назву апки(можна вказати любу назву)":"Android Game Id",
    
  </details>
  
  <details>
    <summary><strong>IS Monetization</strong></summary><br>
  <strong>Копіювання App ID</strong>
    
    1. Відкриваємо IronSorce, тикаємо на Apps
    2. Шукаємо потрібну нам апку
    3. Копіюємо App ID

  <img src="https://github.com/xanet0/Arbitrage-Analitycs-Documentation/blob/main/image/Screenshot_5.png" alt="Фото" style="width: 80%;"><br>

  <strong>Додавання Кампанії в Бота</strong>
  
    1. Заходимо в data.json, шукаємо розділ ironsourceMonet
    2. Далі орієнтуємося по назвам апок і додаємо нову строку, в тому ж порядку як в табличці
    3. В строці пишемо "Назву апки(можна вказати любу назву)":"App ID",
  
  </details>
  
  <details>
    <summary><strong>IS Ads</strong></summary><br>
    
  Примітка: Налаштування IS Ads буде трохи відрізнятися від інших
  <strong>Отримання назви апки в IS Ads</strong>
    
    1. Відкриваємо IronSource, відкриваємо Ads
    2. Тицяємо на Report Generator
    3. Після чого тицяємо на триб
    4. У вас буде стояти галочка на Country, її ми прибираємо. На фотці видно що повинно стояти
    5. Тикаємо на Run Report
  <h1><a href="https://slovnyk.ua/index.php?swrd=%D1%82%D1%80%D0%B8%D0%B1" target="_blank">Триб</a></h1><br>
  <img src="https://github.com/xanet0/Arbitrage-Analitycs-Documentation/blob/main/image/Screenshot_3.png" alt="Фото" style="width: 80%;"><br>

    1. Перед собою ми бачимо список всіх активних кампаній
    2. Далі нам просто потрібно скопіювати назву кампанії

  <img src="https://github.com/xanet0/Arbitrage-Analitycs-Documentation/blob/main/image/Screenshot_9.png" alt="Фото" style="width: 80%;"><br>

  Наступний крок з додаванням Кампанії в Бота трохи відрізняється
  <strong>Додавання Кампанії в Бота</strong>
  
    1. Заходимо в data.json, шукаємо розділ ironsourceAds
    2. Далі заходимо в свою табличку та копіюємо назву листа, для которого налаштовуємо бота
    3. Далі додаємо нову строку, порядок не важливий і в строці пишемо "Назву листа в табличці":"Назва апки IS Ads",

    
  </details>
  
</details>
