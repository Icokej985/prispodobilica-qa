# Prispodobilica — testni centar

Statički portal za ručni QA aplikacije Prispodobilica.

- `index.html` — početna stranica s funkcionalnostima.
- `premium.html` — 144 scenarija Premium QA, vezana uz commit `887fe91`.
- Buduće funkcionalnosti dodavati kao zasebne stranice i skupine, bez promjene postojećih testnih ID-jeva.

## Sigurnost rezultata

Odgovori su samo u lokalnom `localStorage` preglednika. Ne postoji backend, korisnički račun ni sinkronizacija između uređaja. Testni rezultati nisu pohranjeni na GitHub. Obvezno redovito izvoziti JSON sigurnosnu kopiju. Kod prelaska s lokalne `file://` stranice na GitHub Pages potrebno je izvesti JSON na staroj stranici i uvesti ga na novoj.

## Kompatibilnost i buduća proširenja

Premium verzija čuva podatke pod ključem `prispodobilica-premium-qa-887fe91-v2` i provjerava shemu/commit pri uvozu; nemojte mijenjati postojeće ID-jeve ili ključ pri kozmetičkim dopunama. Za novi QA ciklus koristiti novi identitet i predvidjeti migraciju sigurnosnih kopija, bez prepisivanja starijih rezultata.

## Objavljivanje

Ova grana namijenjena je GitHub Pagesu kao izvor `qa-pages` / `(root)`. Sadrži samo statične datoteke portala u svom završnom stablu (bez izvornog Flutter projekta). Korisnik mora ručno omogućiti Pages u postavkama repozitorija ako njegov GitHub plan to dopušta. **Objavljena Pages stranica u pravilu je javno dostupna čak i ako je repozitorij privatan.** Ne dodavati privatne tokene, osobne podatke ili interne tajne. Objavljivanje ne mijenja vidljivost samog repozitorija.

## Pravila rada

Bez promjena odobrenog Flutter UI-ja; ovaj portal je zasebni QA alat. Ne objavljivati nalaze ili osobne podatke automatski. Portal održavati samo u ovom repozitoriju; ne mijenjati privatni repozitorij aplikacije.
