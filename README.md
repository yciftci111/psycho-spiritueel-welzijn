# Psycho-spiritueel welzijn — onderzoeksdashboard

Interactief dashboard bij het masterscriptie-onderzoek naar het **psycho-spirituele welzijn van moslims in Nederland**. Respondenten kunnen via filters zelf zien wat er met de geanonimiseerde data gebeurt: gemiddelden, antwoordverdelingen, betrouwbaarheid, correlaties en groepsvergelijkingen — allemaal live herberekend over de groep die je selecteert.

**N = 353 geldige respondenten** · geen persoonsgegevens of open antwoorden zichtbaar.

## Over de scriptie

| | |
|---|---|
| **Titel** | Religieuze coping, spiritueel welzijn en schadelijke gedachten bij Nederlandse moslims |
| **Ondertitel** | Een kwantitatieve analyse binnen het psycho-spirituele perspectief van Ibn Qayyim al-Jawziyya |
| **Auteur** | Havva Yıldız — BA Islamitische Theologie |
| **Opleiding** | HBO Postinitiële Master Islamitische Geestelijke Verzorging |
| **Instelling** | Islamic University of Applied Sciences Rotterdam (IUASR) |
| **Graad** | Ter verkrijging van de graad doctorandus (drs.) |
| **Studentnummer** | 203774 |
| **Studiejaar** | 2025–2026 |

🔗 **Live:** https://&lt;gebruikersnaam&gt;.github.io/psycho-spiritueel-welzijn/

> Vervang `<gebruikersnaam>` door je eigen GitHub-gebruikersnaam zodra de pagina online staat.

<!-- Tip: voeg een schermafbeelding toe en verwijs ernaar, bijv.:
![Schermafbeelding van het dashboard](docs/screenshot.png)
-->

## Werkt op telefoon, tablet en desktop

Het is één enkel `index.html`-bestand dat zich automatisch aanpast aan de schermgrootte — er zijn dus geen aparte mobiele of tabletversies nodig. Op telefoon en tablet schuiven de filters in als een paneel via de **Filters**-knop rechtsboven; op een breed scherm staan ze permanent in de zijbalk. Alle grafieken, tabellen en de correlatie-heatmap schalen mee.

## Inhoud van het dashboard

Zes tabbladen, die allemaal direct reageren op de filters (geslacht, leeftijd, opleiding, etniciteit, religiositeit, klachten en meer):

| Tab | Wat je ziet |
|-----|-------------|
| **Overzicht** | Gemiddelde score, spreiding en betrouwbaarheid (Cronbach's α) per schaal, plus een korte steekproefbeschrijving |
| **Steekproef** | Verdeling van de respondenten per demografisch kenmerk |
| **Schalen** | Antwoordverdeling per stelling op de 5-punts Likertschaal, met het gemiddelde per item |
| **Correlaties** | Pearson-correlaties tussen de vier schalen, als heatmap |
| **Vergelijken** | Gemiddelde score per groep, met 95%-betrouwbaarheidsinterval — kies zelf kenmerk en schaal |
| **Over** | Verantwoording, methode en uitleg van de begrippen |

## De vier schalen

Elke schaal bestaat uit 10 items op een schaal van 1 (*helemaal mee oneens*) tot 5 (*helemaal mee eens*). Een schaalscore is het gemiddelde van die tien items en ligt dus tussen 1 en 5.

| Code | Schaal | Wat het meet | Cronbach's α |
|------|--------|--------------|:---:|
| **HCO** | Hart-gebaseerde Cognitieve Ontregeling | Verstorende gedachten, mentale afwezigheid, innerlijke onrust | 0.89 |
| **PSC** | Positieve Spirituele Coping | Geloofsgerichte manieren om met stress en tegenslag om te gaan | 0.87 |
| **NSC** | Negatieve Spirituele Coping | Innerlijke twijfel, controleverlies en spanning in de geloofsbeleving | 0.88 |
| **SHB** | Spirituele Hartbalans | Innerlijke rust, zuiverheid en verbondenheid | 0.89 |

Een hogere score betekent telkens méér van het genoemde begrip. Alle vier de schalen zijn intern consistent (α > 0.80).

## Bestanden

```
index.html          het volledige dashboard (de data zit erin ingebouwd)
chart.umd.min.js    grafiekbibliotheek (Chart.js 4.4.1, lokaal meegeleverd)
README.md           dit bestand
```

Er is geen build-stap en geen server nodig. Dubbelklik `index.html` om het lokaal te openen.

## Online zetten met GitHub Pages

1. Maak een repository `psycho-spiritueel-welzijn` aan en upload `index.html`, `chart.umd.min.js` en `README.md`.
2. Ga in de repo naar **Settings → Pages**.
3. Kies bij *Source*: **Deploy from a branch** → branch **main** → map **/ (root)** → **Save**.
4. Na ongeveer een halve minuut staat het dashboard op `https://<gebruikersnaam>.github.io/psycho-spiritueel-welzijn/`.

Via de terminal:

```bash
git init
git add index.html chart.umd.min.js README.md
git commit -m "Onderzoeksdashboard psycho-spiritueel welzijn"
git branch -M main
git remote add origin https://github.com/<gebruikersnaam>/psycho-spiritueel-welzijn.git
git push -u origin main
```

## Data en methode

- In totaal vulden 354 mensen de vragenlijst in. Eén respondent gaf geen toestemming voor deelname en is verwijderd, waardoor **353 geldige respondenten** overblijven, allemaal met volledige antwoorden.
- Scores zijn gemiddelden van tien Likertitems (1–5). Bij filteren en vergelijken worden gemiddelden, spreidingen, betrouwbaarheid en correlaties **opnieuw berekend** over precies de geselecteerde groep.
- Cronbach's α geeft aan hoe consistent de tien items samen één begrip meten; boven 0.80 geldt als goed.

## Let op

- Correlaties beschrijven samenhang, **geen** oorzaak-gevolg.
- Gemiddelden van groepen met minder dan 10 respondenten zijn gemarkeerd en minder betrouwbaar.
- De cijfers zijn beschrijvend; toetsende conclusies staan in de scriptie zelf.
- Er worden bewust geen open tekstantwoorden getoond, om de anonimiteit van respondenten te waarborgen.

## Privacy

Het dashboard toont uitsluitend geaggregeerde, geanonimiseerde resultaten. Er zijn geen herleidbare persoonsgegevens of vrije tekstantwoorden in opgenomen.

## Verantwoording

Dit dashboard hoort bij de masterthesis van **Havva Yıldız** (Islamic University of Applied Sciences Rotterdam, 2025–2026). Suggestie voor verwijzing:

> Yıldız, H. (2026). *Religieuze coping, spiritueel welzijn en schadelijke gedachten bij Nederlandse moslims: Een kwantitatieve analyse binnen het psycho-spirituele perspectief van Ibn Qayyim al-Jawziyya* [Masterthesis, Islamic University of Applied Sciences Rotterdam].
