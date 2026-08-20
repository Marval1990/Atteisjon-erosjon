# Attrisjon og erosjon

Chairside dokumentasjonsverktøy for norske tannleger som skal dokumentere
patologisk tap av tannsubstans (attrisjon/erosjon) opp mot HELFO
innslagspunkt 9.

## Bruk

Åpne `index.html`. Det er alt. Én fil, ingen avhengigheter, ingen CDN,
ingen byggesteg — verktøyet fungerer offline ved å dobbeltklikke filen.
Optimalisert for desktop, 1280 px og bredere.

## Innhold

1. **Grunndata** — alder (obligatorisk), dato, pasientnummer, behandler
2. **TWI-registrering** — odontogram 18–11 / 21–28 / 48–41 / 31–38 etter
   Smith & Knight Tooth Wear Index. Fire flater per tann, klikk for å øke
   score 0–4, Shift-klikk for å gå bakover. Tenner kan markeres som
   manglende og utelates da fra beregningen. Bryter for forenklet modus
   med kun okklusal/incisal flate.
3. **BEWE** — valgfri, kollapsbar. Seks sekstanter, sum 0–18 med risikonivå.
4. **Okklusjon og vertikal dimensjon**
5. **Etiologi og aktivitet** — attrisjon, erosjon, abrasjon
6. **Alvorlighetsvurdering mot innslagspunkt 9** — sjekkliste på sju punkter
   der hvert punkt krever både hake og fritekst. Gir dokumentasjonsstatus
   RØD / GUL / GRØNN.
7. **Behandlingsvalg** — materialvalg, obligatorisk journalføring ved
   kroneterapi, oppbyggingsplan og oppfølging
8. **Generert journaltekst** — sammenhengende norsk journaltekst som ren
   tekst, klar til å limes inn i Opus

Nederst: resultatpanel med begrunnelseslister, kontrollpunkter, «Nullstill»
og «Skriv ut rapport». Sticky bunnlinje viser løpende dokumentasjonsstatus
og antall tenner med dentineksponering.

## Personvern

Ingen data lagres eller sendes. Ingenting skrives til nettleserens lagring,
og verktøyet gjør ingen nettverkskall. Bruk kun pasientnummer — aldri navn
eller fødselsnummer.

## Design

CSS-en er kopiert fra [perioberegning](https://github.com/Marval1990/perioberegning)
slik at de to verktøyene framstår som samme produkt: samme CSS-variabler
(primærfarge `#1E6E5B`, alvorlighetsskalaen `--sev1` til `--sev4`, radius,
fontstack), samme header, nummererte seksjoner med ingress, og de samme
klassenavnene på kort, segmentknapper, skjemakontroller, resultatpanel og
print-CSS.

## Avgrensning

Verktøyet er dokumentasjonsstøtte, ikke en garanti for stønadsrett. Det
inneholder ingen takster, refusjonsbeløp eller pasientbetaling. HELFO
forhåndsgodkjenner ikke kasus — vurderingen gjøres etterskuddsvis, og
bevisbyrden ligger hos behandlende tannlege. Dokumentasjonsstatusen som
vises er verktøyets kontroll av at feltene er utfylt, ikke en godkjenning.
