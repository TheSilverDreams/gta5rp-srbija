---
layout: post
title: "RAGE MP neće da se pokrene? Rešenja za najčešće greške"
description: "RAGE MP ne radi, kraši ili ga blokira antivirus? Prolazimo najčešće greške i rešenja: Defender, administrator, verifikacija fajlova, drajveri i modovi."
date: 2026-05-24
slug: rage-mp-greske
image: /assets/img/ragemp-instalacija.jpg
tags: [gta5rp, ragemp, greske]
---

RAGE MP neće da se pokrene, kraši pri ulasku na server ili se ruši nasred igre? Dobra vest je da se ogromna većina problema svodi na pet-šest poznatih uzroka, i svi se rešavaju kod kuće za nekoliko minuta. Prođi listu redom, poređana je od najčešćeg ka ređem.

Ako klijent još nisi ni instalirao, kreni od [vodiča za instalaciju]({{ '/kako-instalirati-rage-mp/' | relative_url }}), tamo su pokrivene zamke samog postavljanja.

## Antivirus ili Windows Defender blokira klijent

Ubedljivo najčešći krivac. RAGE MP se pri pokretanju kači na proces GTA V, a to je ponašanje koje antivirusna heuristika ume da protumači kao malware. Rezultat: Defender ili antivirus u tišini obriše ili stavi u karantin deo klijenta, pa se RAGE MP ne pokreće, javlja da fajlovi nedostaju ili beskonačno "popravlja" instalaciju.

Rešenje u dva poteza:

1. Dodaj ceo folder RAGE MP (npr. `C:\RAGEMP`) u izuzetke antivirusa. Kod Defendera: Windows Security, Virus & threat protection, Exclusions.
2. Pusti klijent da se sam popravi pri sledećem pokretanju, ili ga reinstaliraj ako je šteta veća.

Bitno: izuzetak dodaj samo ako si klijent skinuo sa zvaničnog sajta rage.mp. Za fajl sa nekog trećeg sajta ovo pravilo ne važi, tu antivirus možda ima pravo.

## Pokreni kao administrator

Klijent tokom rada piše fajlove: update-uje sebe, skida sadržaj servera, pravi keš. Ako je instaliran u Program Files ili Windows steže dozvole, bez administratorskih prava sve to puca na čudne načine: zamrznut update, prazna lista servera, crash bez poruke.

Desni klik na `ragemp_v.exe`, pa Run as administrator. Ako to pomogne, u Properties fajla, kartica Compatibility, štikliraj da se uvek pokreće kao administrator i zaboravi na problem.

## Proveri fajlove GTA V

Ako se igra ruši pri učitavanju ili RAGE MP javlja grešku vezanu za fajlove igre, verovatno je neki fajl GTA V oštećen ili ga je neki mod prepravio. Verifikacija je ugrađena u svaki launcher:

- Steam: desni klik na igru, Properties, Installed Files, Verify integrity of game files.
- Rockstar Games Launcher: Settings, GTA V, Verify Integrity.
- Epic: tri tačke pored igre, Manage, Verify Files.

Provera zna da potraje, ali posle nje imaš čiste fajlove i jednu nepoznatu manje.

## Skini modove iz singleplayera

Ovo je zamka za sve koji su nekad modovali GTA V. Fajlovi tipa `dinput8.dll`, `ScriptHookV.dll`, folder `mods`, grafički modovi poput ReShade ili ENB: sve to živi u folderu igre i svađa se sa RAGE MP. Simptomi idu od crash-a na startu do rušenja tek pri ulasku na server.

Rešenje: izbaci sve modove iz foldera GTA V, pa uradi verifikaciju fajlova iz prethodnog koraka. Ako baš hoćeš da zadržiš singleplayer modove, drži dve kopije igre ili premesti mod fajlove u poseban folder dok igraš multiplayer. Pola posla je znati da RP serveri ionako imaju svoj sadržaj, [BMRP](https://bmrp.rs) na primer sam učitava celu mapu Beograda, tvoji lokalni modovi mu samo smetaju.

## Ažuriraj drajvere grafičke

Zastareli GPU drajveri prave rušenja koja izgledaju nasumično: igra pukne posle pola sata, ekran zamrzne pri teleportu, artefakti na kastom mapama. Skini najnoviji drajver sa sajta NVIDIA ili AMD (ne preko Windows Update, on kasni), instaliraj uz opciju čiste instalacije, restartuj.

Usput proveri i da mašina uopšte guši: ako ti GTA V i inače jedva radi, multiplayer sa stotinu igrača neće pomoći. Šta je realno potrebno imaš u tekstu o [sistemskim zahtevima za RP]({{ '/rage-mp-sistemski-zahtevi/' | relative_url }}).

## Igra nikad nije pokrenuta do menija

Kratko ali često kod novih instalacija: GTA V mora bar jednom da se pokrene do glavnog menija kroz svoj launcher pre prvog starta RAGE MP. Launcher tada završava inicijalizaciju i aktivaciju, bez koje klijent nema ispravne fajlove na koje se kači.

## Ne mogu da se konektujem na server, sve ostalo radi

Ako se klijent uredno pali, ali konkretan server ne odgovara ili te izbacuje pri connectu, problem je najčešće na strani mreže ili servera, ne kod tebe: restart servera, tvoj firewall, pogrešno ukucan IP. Za tu kategoriju problema imaš poseban tekst o [konektovanju na server preko IP adrese]({{ '/kako-se-konektovati-na-server/' | relative_url }}), uključujući šta da proveriš kad server ćuti.

## Kad ništa sa liste ne pomaže

Redosled za tvrdoglave slučajeve: potpuno obriši folder RAGE MP, reinstaliraj sa rage.mp kao administrator u čist folder tipa `C:\RAGEMP`, verifikuj fajlove GTA V, pa probaj ponovo. To resetuje praktično sve što može da se pokvari na tvojoj strani.

Ako ni to ne prođe, pitaj u Discord zajednici servera koji igraš. Na većim projektima ista greška je već viđena sto puta i neko će ti u dve poruke reći šta je. Brže od bilo kog foruma.
