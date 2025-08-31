# SRA Ampumakoe – Single-Page App (SPA)

Pieni selainpohjainen pistelaskuri **SRA-ampumakokeen** tulosten kirjaamiseen ja läpäisyn arviointiin.

Toimii täysin staattisena sivuna osoitteessa https://teemuq.github.io/sra-koe/, ja tallentaa tulokset selaimen paikalliseen muistiin, jotta ammuntaa voi jatkaa osissa.

> ⚠️ **Ei virallinen työkalu.** Tämä on harrastelähtöinen apuväline, eikä takaa oikeita tuloksia. Noudata aina **RESULin** ajantasaisia sääntöjä ja **RO:n** päätöstä.
>
> Kehittäjä/ylläpitäjät eivät vastaa virheistä tai seurauksista.

## Ominaisuudet

- **1–4 ampujaa**; jokaiselle oma tuloskirjanpito.
- **Rastit välilehdillä** (R1–R5) + **Tulos**-välilehti.
- **Nopeat syötöt**: A/B, C, D, ohi sekä aika (desimaalit tuettu).
- **Mukautuva “Täytä: _n_A”** –painike (täyttää sarjan “2A/taulu” tms. rastin laukausmäärän mukaan).
- **R5-valinta**: pistooli (8 ls) tai kivääri (12 ls). :contentReference[oaicite:0]{index=0}
- **Per-ampuja “Suoritus turvallinen (RO hyväksyy)”** -valinta.
- **Tuloksen väri Tulos-välilehdessä**: vihreä = hyväksytty, punainen = hylätty (kun kaikki rastit syötetty).
- **Paikallinen tallennus**: syötöt säilyvät selaimen LocalStoragessa (ei palvelinriippuvuutta).

## Käyttö

1. Lisää ampujat **Asetukset ja ampujat** -paneelista → **Aloita ammunta**.
2. Valitse **R5-ase** (pistooli/kivääri).
3. Syötä jokaisen rastin sarjoihin **A/B**, **C**, **D**, **Ohi**, **Aika (s)**.
4. Siirry **Seuraava rasti →**; viimeiseltä rastilta painike on **Näytä tulokset**.
5. **Tulos**-välilehdellä näet koonnin valitulle ampujalle ja voit merkitä **Suoritus turvallinen**.

## Pistelasku pähkinänkuoressa (appin oletukset)

- **Taulupisteet**: A- ja B-alue 5 p, C-alue 3 p, D-alue 1 p.
- **Pistelaskutapa**: kokeessa käytetään **rajoitettua laukausmäärää**.
- **Rangaistukset (rajoitettu laukausmäärä)**: puuttuvista osumista **ja** ylimääräisistä laukauksista vähennetään **2 × yhden osuman maksimipiste** (paperitaululla 2 × 5 p = **−10**/tapaus).
- **Osumakerroin (HF)** = *pisteet / kokonaisaika*.
- **Hyväksytty koe**: osumakerroin **> 1,3** **ja** suoritus muuten **turvallinen**.

> Huom: jos seurasi käyttää eri tulkintoja (esim. lisäoheistehtäväpisteitä tms.), tarkista laskukaavat RO:lta. SRA-säännökset sallivat eri pistelaskutapoja rasti­kuvauksesta riippuen.
> 
## Tietosuoja

- Kaikki tieto (ampujat, syötöt, valinnat) tallentuu **vain selaimen LocalStorageen**.  
- Appi ei lähetä tietoja minnekään eikä käytä analytiikkaa.

## Lähteet ja viitteet

- **SRA-ampumakoe (2023)** – rastien sisältö, kokonaislaukaukset, maksimipisteet, läpäisy (HF > 1,3) ja turvallisuusvaatimus. 
- **SRA-säännöt (ver. 8.1, 2024)** – taulupisteet (A/B=5, C=3, D=1), pistelaskutavat, rangaistukset rajoitetussa laukausmäärässä (−2×max/osuma → −10/pst), osumakertoimen määräytyminen.

> **Versiot muuttuvat**: varmista aina viimeisin versio RESULin sivuilta ja noudatettava rasti­kuvaus kilpailussa/harjoituksessa.


## Tunnetut rajoitteet

- Tämä laskuri ei huomioi kaikkia mahdollisia rasti-variaatioita (esim. oheistehtäväpisteet).
- Aikarajan ylitysrangaistuksia ei mallinneta erikseen, ellei rasti sitä vaadi. Tarkista rasti­kuvaus.

## Lisenssi

MIT. Soveltuu käytettäväksi “omalla vastuulla”.

