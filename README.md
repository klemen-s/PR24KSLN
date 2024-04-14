## OPIS PROBLEMA
Stanovanjski trg v Ljubljani je kompleksen in se nenehno spreminja. Cene stanovanj se razlikujejo glede na lokacijo, velikost in druge dejavnike. Cilj tega projekta je razumeti, kako se te cene spreminjajo in kaj vpliva na povpraševanje po stanovanjih v različnih delih mesta. S tem bomo lahko bolje razumeli trende na trgu in kaj bi to lahko pomenilo za ljudi, ki jih zanima nakup stanovanja.

## PODATKI
Vir: https://ipi.eprostor.gov.si/jgp/data

Podatki za obdelavo so zajeti v dveh datotekah:
-	ETN_SLO_KUP_LETO_delistavb_20240302.csv
-	ETN_SLO_KUP_LETO_posli_20240302.csv

Za analizo stanovanjskega trga v Ljubljani potrebujemo določen par datotek (ETN_SLO_KUP_LETO_delistavb_20240302.csv in ETN_SLO_KUP_LETO_posli_20240302.csv). 
Preko »ID Posla«, ki je prisoten v obeh datotekah, lahko ugotovimo kater posel je bil kje sklenjen in za katero vrsto objekta gre (stanovanje). Po tem postopku lahko potem izluščimo vse stanovanjske objekte in posle, ki so se zgodili v Ljubljani.
Podatki v določenih primerih niso bili popolni, take primere sva odstranila iz končne množice podatkov.

Končna oblika obdelanih podatkov:
-	 #ID, #Ime ulice, #Hišna številka, #Leto izgradnje stanovanja, #Kvadratura stanovanja, #Datum prodaje, #Cena (EUR)

## GLAVNE UGOTOVITVE
Glavne ugotovitve iz trenutnih podatkov:
-	v Ljubljani je bilo, v zadnjih desetih letih, najmanj stanovanj prodano leta 2018 in 2023.
  ![plot](./assets/pr_projekt_slika_1.png)
  
-	čeprav je bilo v Ljubljani najmanj stanovanj prodano leta 2023, je bilo v tem letu eno stanovanje prodano za največ denarja do sedaj (7, 500,000€).
-	avgust, januar in april so meseci kadar ljudje kupijo najmanj stanovanj v Ljubljani, v zadnjih desetih letih. 

