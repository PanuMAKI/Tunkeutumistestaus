# H1 
## X) Tiivistys
Herrasmishakkerit jakso Niko Nirvi | 0x3f.
  - Podcastin mukaan selaimen laajennuksia ei tarvitse tietoturvan parantamiseksi mutta salasana pankki olisi kaikille erittäin hyödyllinen
  - Vieraan Niko Nirvin mielestä tekoäly ei tule tekemään parempaa peliä kuin ihminen

Hutchins et al 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains, chapters Abstract, 3.2 Intrusion Kill Chain.
  - tekstissä kerrotaan erivaiheet mitä kuuluu kill chainiin.
  - 1 Reconnaissance, 2 Weaponization, 3 Delivery, 4 Exploitation, 5 Installation, 6 Command and Control, 7 Actions on Objectives.

KKO 2003:36.
  - Ennakopäätös Op pankin yritetystä tietomurrosta.
  - käräjäoikeus tostesi syytetyn syylliseksi.
  - hovioikeus myös todennnut syylliseksi ja korkein oikeus yhtyi hovioikeuden päätökseen
  - 


## a) kali linux lataus
versio: 2026.1
Asennus tapa: ISO

## b) VM irrottaminen netistä.

irrotettu vm netistä. 
<img width="356" height="75" alt="Näyttökuva 2026-03-29 210353" src="https://github.com/user-attachments/assets/dbf5ed26-4932-4eb4-9a97-4ec7dc069033" />

## c) Portti skannaus.
ensimmäisessä skannauksessa näkyy että kaikki 1000 porttia on ignored tilassa. Parametri -T4 on nopeuden säätö ja -A on agressive scanning joka antaa laajemman analyysin.

<img width="644" height="276" alt="kuva" src="https://github.com/user-attachments/assets/f4efc245-d933-40ae-87e9-734de7b6539a" />

## d) uusin skannaus demonien kanssa
asensin apache2 ja ssh:n jonka jälkeen skannaus näytti tältä.

<img width="637" height="376" alt="kuva" src="https://github.com/user-attachments/assets/b85bdb76-9aaa-4ada-bee5-0e492ae3ee54" />

Asennuksen jälkeen portit 22 ja 80 olivat auki. 

## e) Hack The Box ratkaisu
<img width="901" height="639" alt="kuva" src="https://github.com/user-attachments/assets/54e00fde-adbd-429d-88e6-52652f1e2d62" />

## lähteet
https://terokarvinen.com/tunkeutumistestaus/
https://lockheedmartin.com/content/dam/lockheed-martin/rms/documents/cyber/LM-White-Paper-Intel-Driven-Defense.pdf chapters Abstract, 3.2 Intrusion Kill Chain.
https://www.finlex.fi/fi/oikeuskaytanto/korkein-oikeus/ennakkopaatokset/2003/36
herrasmieshakkerit.fi jakso, Niko Nirvi | 0x3f.
https://www.kali.org/get-kali/
