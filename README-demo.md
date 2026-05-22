# ALIA Demo — speel-omgeving zonder hardware

Deze map bevat één bestand: **`alia-demo.html`**. Open het in een browser en je
zit in een werkende kopie van het ALIA besturingssysteem, **zonder dat er een
Raspberry Pi of irrigatie-machine aangesloten hoeft te zijn**.

## Wat kan je ermee?

- Klikken door alle tabs (Overzicht, Weekplanner, Handmatige Beurt, Sensoren, Beurten Live, etc.)
- Beurten starten — cycli "draaien" met realistische timing en eindigen met een gesimuleerde meting
- Geleide kalibratie doorlopen (vul zelf "metingen" in, systeem reageert net als echt)
- Tafels en zones aanpassen
- Backup downloaden / terugzetten
- Multi-zone beurten met verschillende smaken
- Service-modus aan/uit (alle tabs zichtbaar)

Alles wat je aanpast wordt bewaard in de browser (`localStorage`). Sluit je het
tabblad? Open het weer en je hebt nog dezelfde data. Wil je opnieuw beginnen?
Klik op **"↻ Reset demo"** in de roze strook bovenaan.

## Hoe hosten via GitHub Pages

1. Maak een nieuwe GitHub repo (publiek of privé met Pages enabled)
2. Upload `alia-demo.html` en hernoem naar **`index.html`**
3. In repo Settings → Pages → Source: "main / root"
4. Wachten een minuutje, dan staat hij op `https://<jouw-username>.github.io/<repo>/`
5. Stuur die link naar je collega

## Hoe testen lokaal

Dubbelklik gewoon op `alia-demo.html` — opent in je standaard browser. Klaar.

## Wat is anders dan productie?

- **DEMO-banner** bovenaan (roze/oranje strook) zodat duidelijk is dat er geen
  hardware is aangesloten
- Geen echte communicatie met een Pi — alle data zit in de browser
- Cycli zijn timing-getrouw maar er stroomt geen echt water
- Slijtage-tellers lopen wel op zodat dat onderdeel realistisch oefent

Versie: **v2026-05-18.l-DEMO**
