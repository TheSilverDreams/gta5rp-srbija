---
layout: post
title: "Kako da podigneš FPS u GTA 5 za RP servere"
description: "GTA 5 optimizacija za RP servere: koja grafička podešavanja jedu FPS, šta da isključiš, kako drajveri i fullscreen mod utiču na performanse."
date: 2026-06-26
slug: gta-5-optimizacija-fps
image: /assets/img/vozila-tuning.jpg
tags: [gta5rp, ragemp, optimizacija]
---

FPS u GTA 5 na RP serveru pada brže nego u singlplejeru, i to nije do tebe. Serveri kao [BMRP](https://bmrp.rs) ubacuju stotine modovanih vozila, kastom mapu i po sto igrača u istom gradu, pa tvoj računar renderuje mnogo više nego što je Rockstar ikad planirao. Dobra vest: par podešavanja pravi razliku od 20-30 frejmova, a većina igrača ih drži na pogrešnim vrednostima.

Pre nego što diraš bilo šta, proveri da li ti mašina uopšte ispunjava [sistemske zahteve za GTA 5 RP]({{ '/rage-mp-sistemski-zahtevi/' | relative_url }}). Ako si ispod minimuma, nikakvo podešavanje neće napraviti čudo. Ako si na granici ili iznad, čitaj dalje.

## Koja podešavanja najviše jedu FPS?

U meniju Settings > Graphics ima dvadesetak klizača, ali četiri stavke nose najveći deo opterećenja.

**MSAA (anti-aliasing).** Najskuplja stavka u celoj igri. MSAA x8 ume da pojede trećinu frejmova u odnosu na isključen. Stavi FXAA na On, MSAA na Off ili maksimalno x2. Slika će biti malo mekša, ali razlika u FPS je ogromna, pogotovo na slabijim karticama.

**Grass (trava).** Na Ultra podešavanju trava je ubica frejmova čim izađeš iz grada. Spusti na Normal ili High. U gradu se razlika skoro ne vidi, a van grada dobijaš 10-15 frejmova.

**Extended Distance Scaling.** Ovaj klizač u Advanced Graphics tabu određuje koliko detalja igra crta u daljini. Na RP serveru sa modovanim vozilima svaki procenat znači dodatne objekte koje kartica mora da drži u memoriji. Spusti ga na nulu ili blizu nule. Isto važi i za Extended Shadows Distance.

**Shadows (senke).** Soft Shadows na Softest ili AMD CHS / NVIDIA PCSS izgledaju lepo na skrinšotovima, a u vožnji ih ne primećuješ. Stavi Shadow Quality na Normal i Soft Shadows na Sharp. To je još 5-10 frejmova.

Ostala podešavanja diraj po potrebi: Post FX na Normal, Reflection Quality na Normal, Population Density i Variety mogu da ostanu na pola. Texture Quality drži na High ako imaš 4 GB VRAM ili više, jer teksture ne troše FPS nego memoriju.

## Zašto RP server traži više od vanile?

Kad igraš singlplejer, igra crta ono što je Rockstar optimizovao godinama. Na RP serveru dobijaš preko toga: kastom modele vozila koji su često teži od originalnih, dodatne objekte na mapi, plus 50-100 igrača čije aute, skinove i animacije tvoj računar mora da sinhronizuje u realnom vremenu. BMRP ima 453+ realnih vozila, i kad se u centru grada skupi ekipa sa tuniranim autima, kartica radi punom parom.

Zato pravilo glasi: podesi grafiku tako da u praznom delu mape imaš bar 70-80 FPS. Kad uđeš u gužvu, padnuće na 40-50, i to je normalno. Ako u praznom delu imaš 45, u gužvi ćeš gledati slajdšou.

## Drajveri i mod prikaza

Zastareli drajver grafičke kartice ume da košta više frejmova nego bilo koje podešavanje. NVIDIA i AMD redovno izbacuju optimizacije, skini najnoviju verziju sa zvaničnog sajta, ne preko Windows Update.

Drugi detalj koji ljudi preskaču: fullscreen protiv borderless. Klasičan Fullscreen daje karticu igri direktno i po pravilu donosi par frejmova više i manji input lag. Borderless Windowed je zgodniji za alt-tab na Discord, ali na slabijim mašinama košta performanse. Ako se boriš za svaki frejm, igraj u Fullscreen. Ako ti mašina ima rezerve, borderless je udobniji za RP jer stalno skačeš između igre i chata.

## Šta još da uradiš pre pokretanja?

Pozatvaraj pozadinske programe. Chrome sa dvadeset tabova, launcheri, overlay aplikacije, sve to jede RAM i procesor koji GTA 5 treba. Pre ulaska na server otvori Task Manager i ugasi ono što ti ne treba. Discord ostavi, on ti treba za komunikaciju, ali mu isključi hardversku akceleraciju u podešavanjima ako si baš tesan sa resursima.

Proveri i da igra stoji na SSD disku. GTA 5 sa HDD-a učitava teksture sporo, pa dobijaš one ružne trenutke kad se zgrade iscrtavaju pred tobom. Na RP serveru sa kastom mapom to je još izraženije.

I na kraju, restartuj RAGE MP klijent posle dužih sesija. Posle par sati igranja memorija ume da se napuni i FPS polako klizi nadole. Izlazak i ponovno konektovanje rešava stvar za minut. Ako klijent tek instaliraš, postupak imaš u vodiču [kako da instaliraš RAGE MP]({{ '/kako-instalirati-rage-mp/' | relative_url }}).

## Koliko FPS je dovoljno za RP?

Ne treba ti 144 frejma za roleplay. RP nije competitive šuter: većinu vremena voziš, pričaš i kucaš. Stabilnih 60 je sasvim udobno, a i 45-50 u gužvi se normalno igra. Bitnija je stabilnost od cifre: bolje zaključanih 60 nego skakanje između 50 i 110.

Ako si podešavanja sredio i FPS je i dalje očajan, problem je verovatno hardver ili nešto u sistemu, a ne igra. A ako tek krećeš u ceo GTA 5 RP svet i još nemaš server, počni od vodiča [kako da počneš da igraš GTA 5 RP]({{ '/kako-poceti-gta-5-rp/' | relative_url }}), pa dođi na [BMRP](https://bmrp.rs) da testiraš te frejmove na mapi Beograda. Uveče zna da bude i po sto ljudi, pa ćeš odmah videti kako ti mašina diše pod pravim opterećenjem.
