# Pakkumised – töö olek ja järgmised sammud

Seda faili loeb Claude igas uues sessioonis automaatselt. Uuenda seda, kui olek muutub.

## Mis selles repos on

- `Asula_14_plaadikulu.xlsx` – Asula 14 komposiitplaatide ja lamellide materjalikulu (leht "Kuluarvutus").
  - Puhas pind 696,84 m², lõikekaoga (5%) 731,68 m², 146 plaati 4200 × 1200 mm.
  - Lamellid 1822,5 jm (290 tk seinal, 115 tk rõdul, pikkus 4500 mm).
  - Lamellide tellimiskogus on määramata: profiili lahtilõike laius on puudu (lahter B31).
  - Rahalist kulu ei ole: ühikuhinnad puuduvad.

## EPR / projektijuhtimise süsteem (auhtec.ee)

- Süsteemi kood **ei ole** selles repos. Kood asub kas mõnes teises GitHubi repos või kohalikus arvutis.
- Probleemid, mida kasutaja kirjeldas (põhjus teadmata, kood nähtamatu):
  1. Projektijuhtimine ei näita täpset kulu.
  2. Materjalivajaduse alla lisatud vaba rida ei võimalda sinna trükkida.
- Lehte `auhtec.ee` ei saa avada: konteineri võrgupoliitika blokeerib domeeni (proxy 403).
  - Lahendus: keskkonna seadetes (Edit → Network access) lisa `auhtec.ee` lubatud domeenide hulka, jäta "Allow package managers" sisse.
  - Kui süsteem nõuab sisselogimist, pane kasutajanimi ja parool keskkonna saladustesse, mitte vestlusesse.

## Lahtised küsimused kasutajale

- [ ] Millises repos (omanik/repo) või millise failina EPR süsteemi kood on?
- [ ] Komposiitplaadi ühikuhind ja lamellide jooksva meetri hind.
- [ ] Profiili lahtilõike laius (mm), et lamellide tellimiskogus saaks arvutada.
- [ ] Kas plaadi laius 1200 mm on kinnitatud?

## Järgmised sammud

1. Saada EPR koodi asukoht või lisa repo `add_repo` abil.
2. Lisa hinnad ja profiili laius kuluarvutusse.
3. Uuri vaba rea sisestamise probleemi süsteemi koodis.
