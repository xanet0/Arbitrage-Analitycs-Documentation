<h1>Гайд з налаштування та використання бота</h1>
<details>
  <summary><strong>!!! Правила використання бота !!!</strong></summary>
  
  1. Ні в якому випадку не можна змінювати порядок таблиць в Google Sheets
  2. Не переставляти/додавати колонки в сторінках
  3. Дивись пункт 1 та 2
  
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
  <summary>Як заповнити таблицю за інший день</summary>
  <h3>В пункті таблиця не заповнилась все розписано</h3>
</details>


<details>
  <summary>Додавання нової апки в табличку</summary>
  <h3>Налаштування:</h3>
  
  1. Відкриваємо наш репозиторій та потрібну нам папку
  2. Відкриваємо data.json
  3. В табличці створюємо новий лист з кампаніями
  4. Колонки з сервісами повинні бути обов'язково в такому ж порядку як на інших листах 

  <details>
    <summary><h3>Обов'язкові правила</h3></summary>
    
  При додаванні кампанії або апки в data.json <strong>дуже важливий порядок</strong>
  Як потрібно додавати кампанію/апку
    
    Наприклад:
        У нас в табличці такий порядок: Gta USSR, GTA Brazil, Gta Mexico
        Ми хочемо додати GTA Brazil в парсер, в data.json повино вийти так:
        "Gta USSR":"fj438djsdkjf2",
        "Gta brazil":"sdlfsu39d",
        "Gta Mexico":"kdsfhs892df"

  <strong>Примітка</strong>

    Якщо ви додаєте апку в табличку в самий кінець списку, то при додаванні строки в data.json кома в кінці не повинна стояти   "Назву апки":"Campaign Set ID"
    Якщо додаєте апку не в кінці списку, то кома повинна ОБОВ'ЯЗКОВО стояти "Назву апки":"Campaign Set ID",
    
  </details>
  <details>
    <summary><h3>Unity Ads</h3></summary>
  <strong>Копіювання Campaign Set ID</strong>
    
    1. Відкриваємо Unity Cloud, User Acquisition
    2. Наводимо курсором на потрібну нам апку
    3. Копіюємо Campaign Set ID:
    
  <img src="https://github.com/xanet0/Arbitrage-Analitycs-Documentation/blob/main/image/Screenshot_4.png" alt="Фото" style="width: 80%;"><br>


  <strong>Додавання Кампанії в Бота</strong>

    
    1. Заходимо в data.json, шукаємо розділ unityAds

      Структура кода в розділі unityAds
      "Назван апки(можна вказати любу назву)":"Campaign Set ID",
    2. Далі орієнтуємося по назвам апок і додаємо нову строку, в тому ж порядку як в табличці
    3. В строці пишемо "Назву апки(можна вказати любу назву)":"Campaign Set ID",
      
  </details>
  
  <details>
    <summary>Unity Monet</summary>
    
    1.
    2.
    
  </details>
  
  <details>
    <summary>IS Monetization</summary>
  
    1.
    2.

  </details>
  
  <details>
    <summary>IS Ads</summary>
    
    1.
    2.
    
  </details>
  
</details>
