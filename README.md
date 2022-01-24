# CISCO-AgazatiGyakorl-s.pka
Csatlakoztass a Home_Router alhálózatába : IP: 192.168.0.1

Csatlakoztass a Home_Router alhálózatában lévő eszközöket megfelelő kábellel egymáshoz. 
  
Kösse össze a Home_Router-t és a Kábel modem-et. 
A Home_PC-t csatlakoztassa a Home_Router 1-es portjába. 
A Home_Server-t csatlakoztassa a Home_Router 2-es portjába. 
A Home_IPPhone-t csatlakoztassa a Home_Router 3-as portjába. 
A Home_Laptop-ban cserélje ki a NIC-et WPC300N Wifi-s kártyára. 
  
A Home_PC-n kérjen IP címet a DHCP szolgáltatótol. Az alapértelmezett átjáró a Home_Router IP címe, böngésző programmal csatlakozzon az eszközhöz, a felhasználó név és a jelszó alapértemezett (admin, admin) 
  
Engedélyezze a Home_Routeren az ISP Vlan-ok használatát, a 3-as portot rendelje a 20-as (Voip) Vlan-hoz. 

A Home_PC-ről pingelje meg a 70.70.70.10-es IP címet. A pingnek sikeresnek kell lennie!
  
Állítsa át a forgalomirányító belépési jelszavát „Almafa12”-re. 
  
A helyi hálózat a 192.168.212.0/26-os tartományban működjön. 
A Home_Router kapja a hálózat első kioszható IP címét.
Konfigurálja a Home_Router DHCP szolgáltatását, az első kiosztható IP a hálózat 10. IP címe legyen. A DHCP-re maximum 50 db eszköz legyen csatlakoztatható.
  
A Home_PC-ről pingelje meg a 70.70.70.10-es IP címet. A pingnek sikeresnek kell lennie! 
Nyissa meg a Home_PC-ről böngészővel az isp.hu-t. A weboldalnak sikeresen meg kell nyílnia! 
  
A Home_Server DHCP-vel kapjon IP címet, de mindig ugyanazt a 192.168.212.42-t. Vegyen fel számára fenntartást "Server" néven a DHCP szerveren. 
  
A Home_Server-en Web szolgáltatást üzemeltet, készítsen port továbbítást a Home_Routeren a TCP, 80-as portra. 
  
A 5 GHz-es Wifi hálózatokat tiltsa le, a 2,4 GHz-es hálózat SSID-je legyen Home, a hitelesítés WPA2 Personal, AES titkosítással, a jelszó „Almafa12”. 
  
A Home_Tablet-en és a Home_Laptop-on konfigurálja a vezetéknélküli hálózat beállításait. 
  
A Home_Router fix IP címmel csatlakozzon az Internetszolgáltatóhoz, ez legyen a 193.41.10.8/24, alapértelmezett átjáró 193.41.10.1, dns szerver 70.70.70.10. 
Konfigurálja ezeket a beállításokat! 
  
A Home_PC-ről pingelje meg a 70.70.70.10-es IP címet. A pingnek sikeresnek kell lennie. 
  
Csatlakozzon az ISP routerhez (193.41.10.1)  a Home_PC-ről Telnet-el vagy SSH-val, felhasználó név és jelszó: admin, és készítsen User_Voip néven DHCP-t a Voip-os eszközök számára. 
A hálózat legyen a 193.41.20.0/24, melynek az első 20 IP címét zárja ki a terjesztésből. 
Alapértelmezett átjáró legyen a 193.41.20.1, dns szerver a 70.70.70.10, domain név isp.hu, telefonközpont ip címe (option 150) 70.70.80.20. 
  
Csatlakozzon a CMS router-hez (70.70.80.20) az ISP router-ről Telnet-el VTY jelszó  „VTYtitok”, a privilegizált mód jelszava  „enaTitok”.
Konfigurálja a nap üzenetét  „Illetekteleneknek a belepes tilos!”.
Konfiguráljon alapértelmezett utat a CMS forgalomirányítón cél címként a 70.70.80.1-es IP címet megadva. 

Vegyen fel felhasználót a CMS-re 15-ös jogosultsági szinttel, felhasználó név és jelszó legyen  „admin”.
Állítsa a domain nevet  „isp.hu”-ra. 
Készítsen 1024 bites RSA kulcsot.
Állítsa be, hogy a forgalomirányító távoli bejelentkezéskor a helyi adatbázis szerint végezze el a hitelesítést és ez csak SSH protokollal történhessen meg.

  
Helyezze be a hálózati adaptert a Home_IPPhone eszközbe, miután a telefon sikeresen regisztrált telefonszámot, hívja fel a 1003-as eszközt. A hívásnak sikeresnek kell lennie! 
  
Nyissa meg az ISP_PC-ről böngészővel a  193.41.10.8-t. A weboldalnak sikeresen meg kell nyílnia! 
  
