# H3 EternalHomework
## x)

## b) porttiskannaus
Aloitin porttiskannaamalla metasploitable koneen komennolla "db_nmap -sV (Metasploitabe ip)" ja sain seuraavan tuloksen jossa näkyy koneen avoimet portit

<img width="1173" height="552" alt="kuva" src="https://github.com/user-attachments/assets/093a91f5-2ae8-4e0f-b8f7-1c3b4ad9aa2f" />

## c) tietojen tarkastelu.
Services komennolla pystyin tarkastella porttiskannauksesta tallennettuja tietoja jotka olivat samat kun äsken tehdyn skannauksen.

<img width="988" height="460" alt="kuva" src="https://github.com/user-attachments/assets/c49d7c7a-05d6-4822-9c1c-ca50b28b7328" />

services komentoa pystyin suodattaa muutamalla tavalla hakemaan tiettyä porttia tai nimeä.
<img width="1048" height="405" alt="kuva" src="https://github.com/user-attachments/assets/7d3d2bc5-1470-4651-a3fe-399407ac79c5" />

## d) internet famous.
exploit haussa löytyi vsftpd backdoor exploit joka on todella vanha exploit jolla pääsee kohdekoneeseen käsiksi. Otin backdoorin käyttöön komennolla "use1"

<img width="1068" height="185" alt="kuva" src="https://github.com/user-attachments/assets/bcaf9105-5076-4a08-b77e-e333ccf4b952" />

## e) Vertailu
"nmap -oA foo" tallentaa tiedoston .xml tai .txt tiedostona.
"db_nmap" tallentaa metasploitin tietokantaan josta helpompi suodattaa tietoa ja etsiä tiettyjä asioita.

## f) Murtautuminen vsftpd
ensin laitoin rhosts metasploitabel koneen ip osoitteen ja lhost oman kali koneen ip osoitteen.

koska aikaisemmin käytin komentoa "use 1" pystyin nyt vain laittamaan exploit komennon jonka tuloksena oli pääsy metasploitable koneen shelliin.

<img width="898" height="113" alt="kuva" src="https://github.com/user-attachments/assets/58c6a0ae-8674-463d-b710-00d7d3c3c0fa" />

## g) lateral movement.

komennolla "cat /etc/shadow" saat listan käyttäjien salasanoista 

<img width="506" height="598" alt="kuva" src="https://github.com/user-attachments/assets/09134da8-75e8-4e43-a76d-7929fe469cec" />

h) toinen tapa.
toiseksi tavaksi valitsin exploit/unix/irc/unreal_ircd_3281_backdoor joka oli mainittu rapid7 metasploitable 2 exploitbility guidessa.

<img width="863" height="231" alt="kuva" src="https://github.com/user-attachments/assets/69ea7664-b09a-414f-b6df-d6e5ea92a31c" />

Valitsin siis oikean exploitin ja laitoin RHOSTS ip osoitteen oikeaksi sekä LHOST ip osoitteen.
tämän jälkeen syötin komennon "exploit" joka avasi uuden yhteyden metasploitable koneeseen.

<img width="853" height="146" alt="kuva" src="https://github.com/user-attachments/assets/64923d77-c664-4659-b8e9-7430ff8464df" />



