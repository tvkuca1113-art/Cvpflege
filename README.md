# Njega u Njemačkoj

Besplatni alati za medicinske sestre, tehničare i njegovatelje iz BiH i regije
koji rade ili žele raditi u Njemačkoj.

**Bez registracije. Bez plaćanja. Uneseni podaci se ne šalju aplikaciji.**

## Šta sadrži

| Fajl | Šta je |
|---|---|
| `index.html` | Početna stranica |
| `lebenslauf.html` | Alat za Lebenslauf i Anschreiben — 12 dizajna, 6 boja |
| `anerkennung.html` | Vodič kroz priznavanje diplome, sa tabelom za svih 16 pokrajina |
| `rjecnik.html` | Stručni rječnik, 143 izraza bosanski–njemački, sa pretragom |
| `privatnost.html` | Kako se postupa sa podacima; mjesto za Impressum |
| `style.css` | Izgled, zajednički za sve stranice |

## Kako radi

Sve je obična HTML stranica bez servera i bez baze podataka. Životopis se
sastavlja i prikazuje **u pregledniku korisnika** — nijedan uneseni podatak se ne
šalje aplikaciji i ništa se ne pamti (nema `localStorage` ni `sessionStorage`).
PDF se pravi kroz štampu preglednika (`Sačuvaj kao PDF`).

Hosting, kao i kod svake stranice, obrađuje uobičajene tehničke podatke o posjeti
(IP adresa, vrijeme, preglednik). To piše u `privatnost.html`.

Zato nema registracije: nema šta da se registruje.

## Pokretanje

Otvori `index.html` u pregledniku. To je sve.

Za objavu na internetu dovoljno je staviti sve fajlove u isti folder na
bilo koji statični hosting (GitHub Pages, Netlify, Vercel, obični web server).
Putanje su relativne, pa radi i u podfolderu.

`rjecnik.py` nije potreban za rad sajta — to je generator koji pravi
`rjecnik.html` iz liste izraza. Pokreni ga samo ako mijenjaš rječnik.

## Prije objave kao komercijalne stranice

`privatnost.html` sadrži označeno mjesto za **Impressum** (odgovorno lice i adresa).
Njemačko pravo ga traži čim stranica ima komercijalnu namjenu. Dok to nije popunjeno,
tamo namjerno ne stoji izmišljeno ime.

## Napomena

Sadržaj je orijentacija, a ne pravni savjet. O priznavanju kvalifikacije
odlučuje isključivo nadležni ured pokrajine u kojoj se predaje zahtjev.
Pravila se mogu promijeniti.

Izvori navedeni u podnožju stranice `anerkennung.html`.
