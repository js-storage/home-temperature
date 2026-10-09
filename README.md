# home-temperature

Webová nástěnka domácího teploměru (ESP8266 + DS18B20). Data se měří každé 2 minuty
a zařízení je posílá do veřejného ThingSpeak kanálu
[3517634](https://thingspeak.mathworks.com/channels/3517634).

**Stránka:** https://js-storage.github.io/home-temperature/

**Druhá stránka – vodoměr, teplá voda (M5Stack Basic):** https://js-storage.github.io/home-temperature/vodomer/
(kanál [3529108](https://thingspeak.mathworks.com/channels/3529108), navíc stav baterie z field7)

- graf teploty za 24 h / 7 dní, maximum, minimum a průměr
- epizody nad prahem (výchozí 35 °C) a typická denní doba překročení
- stav zařízení (poslední odeslání, Wi-Fi, chyby měření, drift hodin)

Stránka je jeden statický soubor (`index.html`) a data čte přímo z ThingSpeak API
v prohlížeči. Neobsahuje žádné klíče. Jiný kanál: `?ch=<id>`, demo data: `?demo`.
