# Analiza stanovanjskega trga v Ljubljani

### Člana skupine
- Klemen Slatnar (klemen-s)
- Lovro Napotnik (Lovroo)

## Opis problema
Stanovanjski trg v Ljubljani je kompleksen in se nenehno spreminja. Cene stanovanj se razlikujejo glede na lokacijo, velikost in druge dejavnike. Cilj tega projekta je razumeti, kako se te cene spreminjajo in kaj vpliva na povpraševanje po stanovanjih v različnih delih mesta. S tem bomo lahko bolje razumeli trende na trgu in kaj bi to lahko pomenilo za ljudi, ki jih zanima nakup stanovanja.

## Podatki
Vir: https://egp.gu.gov.si/egp/

Podatki za obdelavo so zajeti v dveh datotekah:
- ETN_SLO_KUP_2014_zemljisca_20240302.csv
    - Oblika podatkov:
        - ID_POSLA	NUMBER (12)
        - Šifra KO	NUMBER (10)
        - Ime KO	VARCHAR2 (2000)
        - Občina	VARCHAR2 (2000)
        - Parcelna številka	VARCHAR2 (100)
        - Vrsta zemljišča	NUMBER (12)
        - Vrsta trajnega nasada	NUMBER (12)
        - Starost trajnega nasada	NUMBER (5)
        - Prodani delež parcele	VARCHAR2 (255)
        - Opombe o nepremičnini	VARCHAR2 (2000)
        - Površina parcele	NUMBER (10)
        - Pogodbena cena parcele	NUMBER (20,2)
        - Stopnja DDV parcele	NUMBER (12)



- ETN_SLO_KUP_2014_posli_20240302.csv
    - Oblika podatkov:
        - ID Posla	NUMBER (12)
        - Vrsta kupoprodajnega posla	NUMBER (12)
        - Datum uveljavitve	DATE
        - Datum sklenitve pogodbe	DATE
        - Pogodbena cena / Odškodnina	NUMBER (20,2)
        - Vključenost DDV	NUMBER (12)
        - Stopnja DDV	NUMBER (12)
        - Datum izteka lizinga	DATE
        - Datum prenehanja lizinga	DATE
        - Opombe o pravnem poslu	VARCHAR2 (2000)
        - Posredovanje nepremičninske agencije	NUMBER (12)
        - Datum zadnje spremembe posla	DATE
        - Datum zadnje uveljavitve posla	DATE
        - Vrsta akta	NUMBER (12)
        - Tržnost posla	NUMBER (12)

Za analizo stanovanjskga trga v Ljubljani potrebujemo prav ti dve datoteki, ker datoteka ETN_SLO_KUP_2014_posli_20240302.csv sama po sebi ne vsebuje lokacijo na kateri je bil sklenjen posel. Preko "ID Posla", ki je prisoten v obeh datotekah, lahko ugotovimo kater posel je bil kje sklenjen s tem da poiščemo enak "ID Posla".


