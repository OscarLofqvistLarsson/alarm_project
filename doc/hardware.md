- Pyocm lopy4, ca 350 kr, https://pycom.io/product/lopy4/ (lånad från skolan)

- Expansion board 3.0. ca 160 kr, https://pycom.io/product/expansion-board-3-0/ (lånad från skolan)

- PIR rörelsesensor, ca 120 kr, https://www.electrokit.com/produkt/pir-rorelsedetektor/ (lånad från skolan)

- kopplingbräda, ca 80 kr, https://www.kjell.com/se/produkter/el-verktyg/elektronik/elektroniklabb/luxorparts-kopplingsdack-400-anslutningar-2-pack-p36283

- LiPo batteri, ca 70 kr, https://www.electrokit.com/produkt/batteri-lipo-3-7v-380mah/

- Kopplingstråd, ca 40 kr, https://www.electrokit.com/produkt/kopplingstrad-byglar-for-kopplingsdack-mjuka-65st/ 

- Resistorer, ca 30 kr, https://www.electrokit.com/produkt/motstandssats-1r-8r2-x10-120-st/ (lånad från skolan)

- Tempretaursgivare, 20 kr, https://www.electrokit.com/produkt/tmp36-to-92-temperaturgivare/

- Buzzer, 30 kr, https://www.electrokit.com/produkt/summer-4-khz-miniatyr/

Till att börja med har vi en lopy4 och expansion board 3.0. Dessa gör att vi kan kommunicera med LoRa, WiFi, Bluetooth and Sigfox, med denna expansion board kan vi koppla via USB och dumpa program till vår lopy4. Vi använder oss utav WiFi. Bilderna nedan visar vad alla portar har för karaktäristiker samt hur de är kopplade med varandra.

https://i.imgur.com/8MzhJNB.png
https://i.imgur.com/o0KUFuq.png
https://i.imgur.com/udCZtdD.png

PIR-sensorn kopplar vi till VIN som ger oss 5 volt. Den kopplas även till pin x från dess komminications pin som är den mellersta pinnen, på bilden visar vi med en arduino men den funkar lika bra med en pycom enhet och vi använder pin 20 för detta. Slutligen går sensor ner i GND Nedan ser vi bilden på hur kopplingen ser ut.

https://i.imgur.com/zWZqGvV.png

Buzzern kopplas från pin 6 som kommer att ge den den volt som den behöver för att funka korrekt, den kopplas sedan till GND.

https://i.imgur.com/50amxLS.png

Knappen kopplas till 3 volt som kommer in i en av pinnarna tex 1a, strömmen går snätt över knappen och kommer ut i 2b som sedan går i in i en resistor på cirka 1k ohm som sedan går ner i GND. Pinnen 2a går till pin X på vår pycom enhet. På bilden nedan ser vi koppling med en arduino enhet men funkar på samma sätt med en pycom enhet med byta till pin 7.

https://i.imgur.com/YUKob2J.png

Tempretaursgivaren kopplas från tre pinnar, den första går till 3 volt, den högra går till GND och den mellersta är den pinnen som komminucerar och den kopplar vi till pin 16. På bilden nedan ser vi koppling med en arduino enhet men funkar lika bra med pycom enhet då vi använder motsvarande pin på pycom enhet. 

https://i.imgur.com/qC4dno2.png

LiPo-batteri kopplas direkt till JST-PH-kontakten på vår expansion board.

