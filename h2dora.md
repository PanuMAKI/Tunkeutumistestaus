# H2 Dora the Expllora

## x) Tiivistelmä
## DORA and TLPT testing - Lecture for Haaga-Helia on 31 March 2026
  - Tiistaina 31.3 käydyn luonnon kalvot
  - kalvoissa kerrottaan mikä on DORA
  - Miten säädöksien mukaisia testejä suoritetaan.
## DORA (Regulation ... on digital operational resilience for the financial sector) article 26,27
  - TLPT on tehtävä vähintään 3 vuoden välein, ja sen tulee kattaa kriittiset toiminnot oikeissa tuotantojärjestelmissä.
  - Testaukseen sisällytetään myös ulkoistetut ICT-palvelut, mutta vastuu säilyy aina finanssiyrityksellä.
  - Testaajien tulee olla päteviä, riippumattomia ja sertifioituja.
## TIBER-FI procedures and guidelines 5.4.1
 - Red team -testisuunnitelma (RTTP) laaditaan uhkatiedusteluraportin (TTIR) pohjalta ja sisältää realistiset hyökkäysskenaariot sekä testin tavoitteet.
 - Suunnitelma määrittää, miten hyökkäys toteutetaan käytännössä (menetelmät, kohteet ja “flagit”), ja se hyväksytään ennen varsinaisen testauksen aloittamista.


## a) Asenna Metasploitable 2 virtuaalikoneeseen.
sain metasploitablen ladattua netistä löytyvällä ohjeella ongelmitta.

## b) verkko koneiden välille

Laitoin molempien koneiden asetuksiin virtualboxissa Host-only jotta ne saavat yhteyden vain toisiinsa mutta ei nettiin.

## c) Yhteys toisten välillä.

Kuvissa näkyy että koneet saavat yhteyden toisiinsa mutta eivät internettiin.

<img width="609" height="247" alt="Näyttökuva 2026-04-02 212058" src="https://github.com/user-attachments/assets/c734b7f8-cb24-4f88-86bd-a34e985860c3" />


<img width="588" height="159" alt="Näyttökuva 2026-04-02 212618" src="https://github.com/user-attachments/assets/28ee8cec-6e9f-43ac-90e7-e495fc4ccf0c" />

## d) oikean ip:n tarkistaminen.

<img width="643" height="140" alt="kuva" src="https://github.com/user-attachments/assets/fb6912ee-5fd4-477e-b120-f7d31757937a" />

<img width="605" height="443" alt="kuva" src="https://github.com/user-attachments/assets/828b8bf1-b4b6-443c-967b-af42f59cc318" />

## e) Portti skannaus.
Skannaus paljasti että metasploit koneella on useita avoimia portteja kuten portit 21 22 ja 23.

21 on on FTP joka mahdollistaa anonyymin kirjautumisen koneelle.

22 on ssh joka voi aiheuttaa haavoittuvuuden koneelle jos on esimerkiksi heikko salasana

23 telnet on suojaamaton etäyhteys jonka ssh on korvannut koska telnet käyttää suojaamatonta yhteyttä.

## Lähteet
https://terokarvinen.com/tunkeutumistestaus/#aikataulu

https://medium.com/cyber-collective/setting-up-metasploitable-in-virtualbox-on-kali-linux-1d5c3212f7f3




