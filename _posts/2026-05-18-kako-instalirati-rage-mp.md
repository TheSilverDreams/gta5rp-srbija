---
layout: post
title: "Kako da instaliraš RAGE MP: korak po korak"
description: "Instalacija RAGE MP klijenta od download-a do prvog konektovanja na server: šta ti treba, gde se skida, koje greške da preskočiš i kako da uđeš u grad."
date: 2026-05-18
slug: kako-instalirati-rage-mp
tags: [gta5rp, ragemp, instalacija]
---

Instalacija RAGE MP traje desetak minuta i ne traži nikakvo tehničko znanje, ali ima par mesta gde ljudi redovno zapnu: pogrešan sajt za download, antivirus koji pojede fajl, klijent koji ne vidi igru. Ovaj vodič prolazi ceo put od nule do ulaska na server, sa svim tim zamkama usput.

Ako još ne znaš šta je uopšte ta platforma i zašto se RP igra baš na njoj, baci prvo pogled na tekst [šta je RAGE MP]({{ '/sta-je-rage-mp/' | relative_url }}).

## Šta ti treba pre instalacije?

Dve stvari, bez izuzetka:

1. Licencirana GTA V: Steam, Rockstar Games Launcher ili Epic Games verzija. Piratska kopija ne radi i tu nema zaobilaznice, klijent proverava fajlove igre.
2. GTA V pokrenuta bar jednom do glavnog menija. Ovo ljudi preskaču pa se čude: launcher mora da završi prvu inicijalizaciju da bi RAGE MP imao ispravne fajlove na koje se kači.

Ako igru tek kupuješ, uzmi bilo koju verziju, sve tri rade. Za multiplayer ti ne treba GTA+ ni Shark kartice, samo osnovna igra.

## Korak 1: skini klijent sa rage.mp

Jedina prava adresa je zvanični sajt: rage.mp. Na njemu stoji dugme za download Windows klijenta. Sve ostalo, "brže verzije" sa foruma, torenti, fajlovi iz Discord poruka nepoznatih ljudi, preskoči. Klijent je besplatan, pa nema nikakvog razloga da ga tražiš na drugom mestu, a lažne kopije su omiljen način da neko pokupi tvoje naloge.

Skinut installer je mali, par desetina megabajta. Pravi sadržaj se povlači kasnije.

## Korak 2: instalacija

Pokreni installer desnim klikom, pa "Run as administrator". Nije uvek obavezno, ali štedi glavobolje sa dozvolama kasnije.

Kod izbora foldera važi jedno pravilo: ne instaliraj RAGE MP u folder GTA V, niti u Program Files ako možeš da biraš. Najčistije je nešto tipa `C:\RAGEMP`. Klijent voli da ima svoj prostor gde može slobodno da piše fajlove servera.

Ako Windows Defender ili antivirus u ovom trenutku digne uzbunu, to je poznata priča: klijent se ubacuje u proces igre i heuristika to ume da protumači kao pretnju. Fajl skinut sa rage.mp je bezbedan, dodaj folder klijenta u izuzetke antivirusa. Ako blokada ipak nešto pojede pre nego što si stigao da reaguješ, reinstaliraj, spisak ovakvih problema sa rešenjima imaš u tekstu o [najčešćim RAGE MP greškama]({{ '/rage-mp-greske/' | relative_url }}).

## Korak 3: prvo pokretanje

Pokreni `ragemp_v.exe` iz foldera gde si instalirao (i njega prvi put kao administrator). Klijent će sam da se update-uje na najnoviju verziju, pa da potraži GTA V na disku. Ako je ne nađe automatski, pokazaćeš mu putanju do foldera igre ručno, to je folder u kome stoji `GTA5.exe`.

Kad sve prođe, dobijaš glavni prozor sa listom servera. To je znak da je instalacija gotova.

## Korak 4: konektovanje na server

Imaš dva puta. Prvi je browser servera: skroluj listu, filtriraj, klikni na server koji te zanima. Drugi je Direct Connect, gde ukucaš IP adresu i port direktno. Za srpski RP na mapi Beograda, [BMRP](https://bmrp.rs) se nalazi na adresi `beograd.bmrp.rs:22005`, a možeš ga naći i pretragom u listi.

Prvi ulazak na bilo koji veći server znači download njegovih fajlova: skripte, modeli, kod mape. Kod servera sa kastom sadržajem to ume da bude više gigabajta, pa prvi connect na sporijem netu slobodno ostavi da radi uz kafu. Svaki sledeći ulazak ide za par sekundi. Detaljnije o direktnom konektovanju i šta da radiš kad server ne odgovara imaš u posebnom tekstu o [konektovanju preko IP adrese]({{ '/kako-se-konektovati-na-server/' | relative_url }}).

## Šta posle konektovanja?

To više ne zavisi od RAGE MP nego od servera. Ozbiljni projekti traže registraciju, na BMRP je to nalog na bmrp.rs, pa te kroz kreaciju lika i tutorijal uvedu u grad. Pročitaj pravila servera pre nego što kreneš da se igraš, ban zbog gluposti u prvih sat vremena je klasika koju lako izbegneš.

## Brza provera ako nešto ne radi

Tri najčešća krivca, redom kojim da ih proveriš:

1. Antivirus je blokirao ili obrisao deo klijenta. Izuzetak pa reinstalacija.
2. Klijent nije pokrenut kao administrator, pa ne može da piše fajlove.
3. GTA V nikad nije pokrenuta do menija, pa fajlovi igre nisu kompletni.

Ako ni to ne pomogne, imaš ceo tekst posvećen [rešavanju RAGE MP grešaka]({{ '/rage-mp-greske/' | relative_url }}). U devet od deset slučajeva problem je neki od ova tri i rešava se za pet minuta. Vidimo se u gradu.
