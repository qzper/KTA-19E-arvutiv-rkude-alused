# KTA-19E-arvutiv-rkude-alused

1. ülevaade kursuses kasutatud käsurea programmide ja näidete kohta.
- ping -c *count* *host_name* - saadab signaali *host*'ini ja ootab vastust
- printf - prindib päringu
- netcat - (nc) on arvuti võrgu tarkvara lugemaks või kirjutamaks võrgu ühendustele
- nc -l *pordi_nr* - netcat kuulab määratud porti
- nc *localhost* *pordi_nr* - saab päringuid määratud saatja määratud pordilt
- ^D - netcat lõpetab ühenduse pordiga
- ^C - lõpetab päringu
- host *hosti_nimi* - gets hosts *alias*'e ja IP-aadressid
- dig *hosti_nimi* - pärib hosti *alias*'e, CNAME-i, IP-aadressid, millisesse serverisse, millal vastas jms
- ip addr show - näitab, mis liidesed (ethernet: eth0, wifi: wlan0, loopback: lo) sinu seadmel on
- ip route show default - näitab vaikimisi *gateway*'d
- sudo tcpdump -n host *hosti_nimi* - lubab kasutajal läbiminevaid ühendusi püüda (minevaid, tulevaid, ning pikkust) 
- traceroute *hosti_nimi* - näitab ühenduslinke sinu ja määratud hosti vahel
2. Ülevaade põhilistest võrguseadmetest ja nende ülesannetest:
 - ruuter (router)  
 Seade, mis ühendab omavahel kaht või enamat arvutivõrku, ning võimaldab nendevahelise andmeside.  
 - kohtvõrgu kommutaator (switch)  
 Arvutivõrgu seade, mille abil luuakse ühendused koht- ehk LAN-võrgus.  
 - tulemüür (firewall)  
 Tarkvara või seade, mis turvakaalutlustel piirab ja reguleerib võrguliiklust arvutivõrgus või võrkude vahel vastavalt määratud reeglitele.  
 - WiFi tugijaam (WiFi access point)  
 Võrgu seade, mis lubab WiFi seadetel ühenduda juhtmega võrku. WiFi tugijaam ühendub tavaliselt ruuteriga, kuid võib olla ka ruuteri osa.  
3. Võrguprotokollid ja nende kasutus (lühidalt):
- SSH  
Turvakest (inglise keeles Secure Shell) on krüptograafiline võrguprotokoll turvaliseks võrguteenuste opereerimiseks turvamata võrgu kaudu. Põhiliselt kasutavad seda arvutikasutajad arvutisüsteemidesse kaugsisselogimiseks.
- telnet   
TCP/IP-il põhinev võrguprotokoll, mis pakub kahesuunalist interaktiivset suhtlusteenus  
- IMAP, POP3, SMTP  
IMAP - põhiliseim meili vastuvõtmise protokoll. IMAP sünkroniseerib sõnumid kõikide seadmete vahel.  
POP3 - samuti meili vastuvõtmise protokoll, kuid ühe seadme jaoks, kus meil võetakse vastu ja kustutatakse serverist. 
SMTP - protokoll meili saatmiseks  
- SNMP  
Protokoll informatsiooni haldamiseks ja monitoorimiseks võrgus. Kasutatakse pigem LAN-is.  
- HTTP, HTTPS  
HTTP on hüperteksti edastus protokoll, mida kasutatakse protokoll teabe edastamiseks arvutivõrkudes. HTTP on alus andmete edastamiseks veebis.  
HTTPS on turvaline versioon HTTP-st, mis kasutab turbeprotokolle TLS/SSL.  
- DNS  
Internetiteenus, mis teisendab domeeninimed internetis või intranetis kasutatavateks IP-aadressiteks või vajadusel ka vastupidi.  
- NTP  
Protokoll täpse aja edastamiseks ajaserveritest.  
- IP  
Arvutivõrgus asuva seadme identifikaator ehk seadmele määratud alaline või ajutine tunnusnumber, mille abil võrku ühendatud seadmed üksteist leiavad.  
- IPv6  
Andmesideprotokoll, mis on loodud praegusel ajal üldkasutatava Internetiprotokolli IPv4 asendamiseks. Praegune IPv4 aadress koosneb neljast kümnendarvust vahemikus 0–255, mis on eraldatud punktidega (näiteks 195.10.0.213). IPv6-aadressid jagatakse kirjutamisel tavaliselt 16-bitisteks rühmadeks, eraldades need kooloniga. Pv6-aadresse kirjutatakse kuueteistkümnendarvudena (näiteks 2002:EF9A:1FFF:93:FEB0:0:0:2ADF).  
- TCP 
Levinuim transpordikihi võrguprotokoll, mida kasutatakse TCP/IP võrkudes. TCP-protokolliga saadetavaid pakette toimetab edasi võrgukihi protokoll, milleks on üldjuhul internetiprotokoll (IP). TCP/IP mudeli järgi on loodud enamik arvutivõrke.  
- UDP  
Transpordikihi andmesideprotokoll, mis on defineeritud IP-ga sõnumite saatmiseks.  
- ICMP  
Andmesideprotokoll, mille abil võrguseadmed vahetavad oleku- ja veainformatsiooni.  
4. Diagnostika vahendid:
- Wireshark
- tcpdump 
- ping 
- traceroute / tracert
- nslookup / dig
- Ressource monitor (Windows)
- netstat 
