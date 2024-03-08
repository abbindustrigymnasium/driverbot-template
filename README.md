# Driverbot template
I det här repot hittar ni exempel kod att utgå från samt instruktioner när ni kodar i ert projekt.

## Mikrokontroller
### Koppla och testa!
Bilden nedan visar hur du ska koppla motorn till din esp.
![image](https://github.com/abbindustrigymnasium/driverbot-template/assets/22837762/703aad4b-4015-4c4a-9739-1644a61969b3)

### Koda
När du löser uppgifterna nedan utgår du från koden i _motorTest.ino_. Börja med att planera dina lösningar mha psuedokod och/eller diagram innan du skriver den faktiska koden.

1. Läs och tolka koden - vad tror du att den gör? Kommentera i filen. Testa att köra koden för att kontrollera dina antaganden.
2. Koden fungerar inte helt som vi tänkt oss, vi vill att den ska byta körriktning efter 2200 millisekunder och efter 2200 byter igen. I nuläget kör den bara åt ett hål, lös det! Utgå från det du lärde dig om koden i steg 1 och experimentera vid behov vidare genom att ändra olika värden för att se vad varje del gör.
3. Gör om kodstrukturen genom att skapa en funktion/metod _Drivetest(input1, input2)_ som utför koden från steg 2. Ett anrop av funktionen kan se ut som nedan.
```
Drivetest(motorPinRightDir, motorPinRightSpeed);
```
4. Nu ska vi utöka funktionaliteten i _Drivetest()_. Kopiera funktionen och döp den nya varianten till _Drivetest2()_. Nu vill vi se hur snabbt och långsamt motorn kan köra. Skapa en loopande funktion där motorns hastighet succesivt ökar.
5. Vi fortsätter bygga ut funktionaliteten! Utgå från _Drivetest2()_ och skapa en ny funktion som vi kan kalla _Drivetest3()_. Den nya funktionen ska kunna göra samma sak som tvåan men alterera mellan vänster och höger varv. Först från långsamt til snabbt på högervarv sedan samma åt vänster sedan höger igen o.s.v...
6. Vi fortsätter bygga på funktionen! I denna version ska du mellan varje varv låta motorn vila några sekunder, du vill även att den i loggen räknar upp hur många varv den har kört.
