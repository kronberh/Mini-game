# Mini-game
Ця міні-гра заснована на PHP і відбувається на сторінці /index.php?page=game1. Гра має двох персонажів: гравеця та комп'ютер (система). Обидва персонажі мають початкову кількість життів, яка задається змінною $basehp і за замовчуванням дорівнює 10.
Користувач вводить число від 1 до 3 через форму на веб-сторінці, відправляючи свій вибір на сервер. Відповідь сервера генерується випадковим чином також від 1 до 3. Результат битви залежить від порівняння числа, введеного користувачем, та числа, згенерованого сервером:
•	Якщо числа збігаються, з життів гравця віднімається випадкова кількість від 1 до 4.
•	Якщо числа не збігаються, втрати зазнає комп'ютер в аналогічному обсязі.
Гра триває до тих пір, поки один з персонажів не втратить всі свої життя (стає 0 або менше). У цьому випадку здійснюється переадресація на сторінку /index.php?module=games&page=game1over, де оголошується переможець гри.
На кожному кроці гри користувачеві надається повна інформація про поточний стан життів кожного персонажа, завдану шкоду та хід битви. Існує також можливість почати гру заново з поверненням до первісного стану життів.
Цей сценарій дозволяє легко адаптувати параметри гри, змінюючи базову кількість життів, що робить гру гнучкою та налаштовуваною.
