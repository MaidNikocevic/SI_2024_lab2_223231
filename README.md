# Втора лабораториска вежба по Софтверско инженерство
## Маид Никочевиќ 223231
### Control Flow Graph

![FINALNO](https://github.com/MaidNikocevic/SI_2024_lab2_223231/assets/164071606/27abb27e-214a-4ced-829d-8414a338e602)
### Цикломатската комплексност
Цикломатската комплексност на дадениот Control Flow Graph е 10, бројот го добивам во формулата:(бр. ребра - бр. јазли) + 2
### Сите тест случаи според Every Branch критериумот
Во следните сценарија за тестирање, можеме да го постигнеме минималниот број на тест случаи според Every Branch. Во првиот случај, кога името не е внесено и потоа се сетира на "unknown", а останатите параметри се валидни (уплатена сума: 100, враќа true). Во вториот случај, првиот елемент во листата е целосно валиден, додека вториот има баркод што почнува со 0, уплатената сума е 50 и враќа false, бидејќи уплатената сума е поголема од вкупната цена на предметите. Во третиот случај, кога листата е null, фрла исклучок веднаш на почетокот на функцијата, без конкретно значење на payment. Четвртиот случај е со елемент без баркод, што исто така предизвикува исклучок, без значење на payment. Во петтиот случај, кога имаме елемент со невалиден карактер во баркодот, се фрла исклучок, пак без влијание од payment.
### Сите тест случаи според Multiple Condition критериумот за условот if (item.getPrice() > 300 && item.getDiscount() > 0 && item.getBarcode().charAt(0) == '0').
TTT - кога цената > 300, има попуст и баркодот започнува со '0'.
TTF - кога цената > 300, има попуст, но баркодот не започнува со '0'.
TFX - кога цената > 300, но нема попуст.
FFX - цената < 300.
