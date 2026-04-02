# H2 Dora the Expllora

## x)

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





