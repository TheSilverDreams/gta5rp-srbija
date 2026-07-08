---
layout: post
title: "Kako da se konektuješ na RAGE MP server preko IP adrese"
description: "Direct Connect u RAGE MP objašnjen na primeru: kako uneseš IP i port, sačuvaš server u favorite i šta da proveriš kad server ne odgovara na konekciju."
date: 2026-06-02
slug: kako-se-konektovati-na-server
image: /assets/img/ragemp-instalacija.jpg
tags: [gta5rp, ragemp, balkan]
---

Konektovanje na RAGE MP server preko IP adrese je najbrži i najsigurniji način da uđeš tačno tamo gde si krenuo. Lista servera u klijentu je duga, imena se ponavljaju i lako je promašiti, a IP adresa ne laže: ukucaš je jednom i ulaziš na pravi server svaki put. Ceo postupak traje pola minuta, a ovde je i šta da radiš kad nešto zapne.

Podrazumevam da RAGE MP već imaš instaliran. Ako nemaš, prvo prođi kroz [vodič za instalaciju]({{ '/kako-instalirati-rage-mp/' | relative_url }}), pa se vrati.

## Šta je uopšte ta adresa?

Adresa RAGE MP servera ima dva dela: host i port, razdvojene dvotačkom. Host je ili domen ili sirova IP adresa, a port je broj koji kaže na koja "vrata" servera kucaš. Primer sa kojim ćemo raditi je adresa srpskog [BMRP servera](https://bmrp.rs):

`beograd.bmrp.rs:22005`

Ovde je `beograd.bmrp.rs` host, a `22005` port. Oba dela su obavezna. Najčešća greška početnika je da ukucaju samo host bez porta, pa se čude što konekcija ne prolazi.

Adresu servera uvek uzimaj sa zvaničnog sajta ili Discorda projekta. Adresa sa nasumičnog foruma može da bude zastarela, a u gorem slučaju i lažni server koji peca naloge.

## Direct Connect, korak po korak

1. Pokreni RAGE MP klijent.
2. U glavnom prozoru nađi opciju Direct Connect (polje za unos adrese, obično uz listu servera).
3. Ukucaj host u polje za adresu i port u polje za port: `beograd.bmrp.rs` i `22005`. Ako klijent nudi jedno polje, ukucaj sve zajedno sa dvotačkom.
4. Klikni Connect.

Prvi ulazak na server znači download njegovog sadržaja: skripte, modeli, kod servera sa kastom mapom i cela mapa. To ume da bude više gigabajta i na sporijem netu traje, pusti ga da završi. Svaki sledeći ulazak ide za par sekundi, jer je sadržaj već na disku.

Kad se učitavanje završi, preuzima te server: login ili registracija, kreacija lika, tutorijal. Na ozbiljnim projektima nalog praviš na sajtu servera, za BMRP je to registracija na bmrp.rs.

## Sačuvaj server u favorite

Da ne kucaš adresu svaki put: u browseru servera unutar klijenta nađi svoj server (posle prvog konektovanja obično stoji u kartici sa istorijom) i klikni na zvezdicu ili opciju za favorite. Sledeći put ga imaš na vrhu, jedan klik i unutra si.

Mali savet uz to: proveri da se ime servera u favoritima poklapa sa onim što očekuješ. Popularnim serverima se ponekad pojave imitatori sličnog imena u javnoj listi, favorit sačuvan sa tačne IP adrese te toga rešava zauvek.

## Server ne odgovara: šta da proveriš

Kad connect ne prolazi, uzroci se dele na tri grupe. Idi ovim redom.

Prvo, tvoj unos. Proveri slovo po slovo host i port, višak razmaka ili tačka umesto dvotačke su klasika. Proveri i da li ti radi internet, zvuči glupo, ali browser koji radi ne znači da ti neka mreža ne blokira gejming portove (školske i poslovne mreže to vole).

Drugo, server. Serveri imaju restarte, tehničke pauze i update-ove, i tada ne primaju konekcije po pravilu nekoliko minuta. Pre paničenja otvori Discord ili sajt servera: ako je restart u toku, tamo već piše. Ako pola grada čeka sa tobom u Discordu, problem definitivno nije kod tebe.

Treće, tvoja mašina. Firewall ili antivirus mogu da blokiraju baš mrežni deo klijenta i kad se sve ostalo uredno pokreće. Dodaj RAGE MP u izuzetke, probaj restart klijenta i rutera. Ako se klijent uz to čudno ponaša i van konektovanja, prođi kroz tekst o [najčešćim RAGE MP greškama]({{ '/rage-mp-greske/' | relative_url }}), tamo je cela dijagnostika.

Ako si sve prošao i dalje ne radi samo taj jedan server, a drugi rade: sačekaj sat vremena ili pitaj u Discordu servera. Uzrok skoro sigurno nije na tvojoj strani.

## Zašto uopšte IP, a ne lista?

Zato što je precizno. Lista servera je odlična za razgledanje, ali kad znaš gde ideš, IP je adresa bez zabune: nema sličnih imena, nema imitatora, nema skrolovanja. Zato serveri i objavljuju adresu na svom sajtu kao zvanični ulaz.

A ako još biraš gde ćeš da igraš, pre kucanja bilo koje adrese pogledaj [pregled RAGE MP servera na Balkanu]({{ '/rage-mp-serveri-balkan/' | relative_url }}) da znaš šta te gde čeka. Kad odlučiš, postupak je isti kao gore: adresa, port, connect, i vidimo se u gradu.
