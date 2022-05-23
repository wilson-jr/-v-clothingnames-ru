# v-clothingnames russian localization

Переведенные на русский язык названия предметов одежды GTA V.

Многие предметы называются как "NO_LABEL" и "NULL", что, вероятно, означает, что они не доступны для покупки в магазинах одежды GTA Online или они достаточно стары, чтобы их имена были закодированы.

Файлы без префикса (т.е. masks.json) предназначены для **mp_m_freemode_01** и **mp_f_freemode_01**.

Файлы с префиксом **male_** предназначены для **mp_m_freemode_01**.

Файлы с префиксом **female_** предназначены для **mp_f_freemode_01**.

Файлы с префиксом **props_male_** предназначены для **mp_m_freemode_01**.

Файлы с префиксом **props_female_** предназначены для **mp_f_freemode_01**.



Files without a prefix (e.g. masks.json) are the clothing items for both **mp_m_freemode_01** and **mp_f_freemode_01** models.

Зайдите на https://wiki.rage.mp/index.php?title=Clothes чтобы увидеть изображения.

# JS Example

```js
// Getting the name of https://wiki.rage.mp/images/c/c2/Clothing_M_11_70.jpg
const maleTops = require("./male_tops.json");
const clothingID = 70;
console.log(`Название предмета: ${maleTops[clothingID][0].Localized}`); // Выходит: "Название предмета: Коричневый кожаный меховой жакет"

// Перечисляются все вариации предметов одежды
Object.keys(maleTops[clothingID]).forEach(variation => {
    console.log(`Вариация ${variation} - ${maleTops[clothingID][variation].Localized}`)
});

/*
    Выходит:
    Вариация 0 - Кожаный меховой жакет — коричневый
    Вариация 1 - Кожаный меховой жакет — рыжевато-коричневый
    Вариация 2 - Кожаный меховой жакет — черный
    Вариация 3 - Кожаный меховой жакет — охра
    Вариация 4 - Кожаный меховой жакет — белый
    Вариация 5 - Кожаный меховой жакет — леопардовый
    Вариация 6 - Кожаный меховой жакет — осенний
    Вариация 7 - Кожаный меховой жакет — хантер
    Вариация 8 - Кожаный меховой жакет — серый
    Вариация 9 - Кожаный меховой жакет — полностью черный
    Вариация 10 - Кожаный меховой жакет — бордо
    Вариация 11 - Кожаный меховой жакет — темно-серый
*/
```
