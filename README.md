Här är en lista på de “Issues” du ska skapa i ditt repo på Github. 

Varje Issue får ett nummer som du kan använda i VS code när du commit:ar. 
[https://code.visualstudio.com/blogs/2020/05/06/github-issues-integration](url)

E:
- [ ] Send fuel gauge, battery and temperature data to AIO.
- [ ] Deep sleep fixed time 10 minutes.
- [ ] Avbryt om man inte får kontakt med WiFi på 10 försök, sov 1 minut.
- [ ] Blinka LED på olika sätt vid a) försöker koppla upp sig b) uppkopplad. Gör en egen funktion blinkLED(times, speed).
- [ ] Versionskontroll via Github. Jag fixar ett repo när du har ett github-konto.

D:
- [ ] Löda OLED
- [ ] OLED med auto-off. Visa namn och datan i textsize 2 på två "frames" i 1,5 sekunder vid Reset-tryck.
- [ ] Ta  hänsyn till om fuelgauge.begin() inte funkar, försök några gånger med kort sleep emellan. Meddela på OLED om det inte lyckas. (Se nedan)
- [ ] Variabel sleep time m.a.p. batteriprocent. 
> - Under 3%: 20 minuter. 
> - 3-6 %: 15 minuter. 
>  - Annars 10 minuter.
- [ ] Dela dina feeds på AIO med mig. AIO användarnamn: **axelmagnus**

C:
- [ ] Löda INA219
- [ ] Löda laddare
- [ ] INA219 laddningsmätare, medelvärde på 1000 samples, skicka upp till AIO.
- [ ] OLED med typsnitt. Välj själv vilket.
- [ ] External Wake up med knapp. Visa data på OLED utan att skicka
- [ ] Skicka data med konstant interval med sleep, trots ev. knapptryck. Se info på Classroom.

B:
- [ ] Om  spänningen är väldigt låg, (<3.4 V), ska den inte försöka sätta i gång WiFi, utan gå tillbaka i sleep och bara ladda batterier.
- [ ] Ta hänsyn till att om någon av dina I2C komponenter inte lyckas starta (.begin() ), försök några gånger med kort sleep, och sedan skicka RTC-lagrade värden i stället.
- [ ] Längre sleep time mellan 18-06, hämta tid från AIO. Se info på Classroom.

A:
- [ ] Skicka meddelande om batteriet understiger viss nivå (<3.4 V). Se [IFTTT](https://learn.adafruit.com/using-ifttt-with-adafruit-io/ifttt-to-adafruit-io-setup).
- [ ] Menysystem för filamentvåg. Helt separat kodfil. Se [Buttons](https://learn.adafruit.com/arduin-o-phone-arduino-powered-diy-cellphone/arduin-o-phone-sketch)
