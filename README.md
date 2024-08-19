# Opgavebeskrivelse

Du er ansat som udvikler i et webbureau. Du indgår i et udviklingsteam, der består af en designafdeling og en kodeafdeling. Bureauet har fået en ordre på et website fra en virksomhed. Layoutet og sitets generelle struktur er allerede fastlagt og godkendt af kunden. Din opgave bliver at udvikle sitets frontend.

Bagtanker er et nyopstartet bageri som tilstræber en stærk online profil og en tæt interaktion med deres brugere. Deres speciale er surdejsbrød og bageriet deler deres opskrifter og vil gerne have brugernes feedback i form af kommentarer.

Mediegrafikeren har leveret et godkendt design, som du skal sætte sitet op efter.

## Kravspecifikation

På de følgende sider gives et overblik over krav til websitets layout, funktionalitet og indhold.

### Generelle krav

- Sitet skal opbygges i HTML, prekompileret CSS og Javascript. Du må gerne anvende et framework eller lignende værktøjer indenfor en eller flere af de tre teknologier.
- Sitet bygges i standardmål efter layoutet.
- Sitet skal være responsivt.
- Sitet skal opfylde de gængse standarder indenfor semantisk, korrekt kode og søgemaskineoptimering (SEO).
- Sitet skal indeholde fejlhåndtering på alle relevante fejl, så brugeren får en fejlmeddelelse der tager hensyn til sitets indhold.
- Der skal være validering på alle formularer/inputelementer.

### Faste elementer

Med undtagelse af forsiden, skal følgende elementer være til stede på alle sider:

- Header med logo og burgermenu til sidebar. Logo skal linke til forside.
- Navigation med produktkategorier og aktiv markering.
- Højre stillet sidenavigation med overordnede punkter: Forside, Produkter, Nyheder, Kontakt og Login. Sidenavigationen kaldes fra et navbar ikon og lukkes på et kryds ikon.
- Brødkrumme
- Footer med logo, adresse og tilmelding til nyhedsbrev

### Forside

Forsiden vises med et logo i toppen og et navbar ikon i højre side. Burgermenuen skal aktivere en sidenavigation som skal animeres ind fra sitets højreside.

Til venstre for midten skal der være en nyhedsboks med fire tilfældige nyheder vist med dato, overskrift og teaser. Ved klik på en nyhed videresendes man til den pågældende nyhed i en detaljevisning.

Som baggrund skal der vises et slideshow i fuld skærm med udvalgte billeder, hvor hvert billede vises i 10 sekunder hvorefter der skiftes til et nyt. I bunden af slideshowet skal det være muligt at navigere imellem de enkelte slides i form af en række klikbare cirkler.

**NB:** I designet skifter alle elementer i slideshowet – det skal kun være baggrundsbilledet.

### Produktliste

Der skal være en side der kan vise lister af produkter ud fra den kategori man klikker på i navigationen i toppen. Den første kategori vises som standard. Den aktuelle kategori skal markeres.

Produkterne vises i en tospaltet kolonne med billede, titel, teaser, knap til at læse mere, antal likes og et hjerteformet like knap.

I toppen skal det være muligt at sortere listen alfabetisk og efter popularitet.

### Produktdetaljer

Sitet skal have en side der kan vise et produkts detaljer titel, billede og tekst. Til højre skal der være en boks med opskrift og en like knap.

Under dette skal der være en liste med bruger kommentarer og mulighed for at skrive en kommentar. Brugere skal være logget ind for at tilføje en kommentar.

### Nyheder

Nyhedsiden skal vises med en aktiv nyhed i venstre side og en liste over nyheder i højre side.

Den aktive nyhed vises med overskrift, dato, billede og brødtekst og nyheder i listen vises i en boks med dato og overskrift. Den aktuelle nyhed markeres med en baggrundsfarve.

### Kontakt

Der skal være en side med en formular og et kort over bageriets lokation.

Hvis formularen er udfyldt korrekt, sendes data til tabellen `messages` i API’et og derefter sendes brugeren videre til en svarside med en besked om at deres data er modtaget.

### Login

Login siden skal give brugere mulighed for at logge ind med deres brugernavn og password.

Når en bruger er logget ind, skal det markeres på sitet. Det er op til dig som udvikler hvordan du vil markere dette.

Desuden skal det være muligt at brugere kan tilgå Min side hvorfra det skal være muligt at administrere kommentarer.

Det skal også være muligt at logge ud.

### Tilvalg til opgaven

Du skal vælge en af følgende tilvalgsopgaver. Du må gerne vælge flere men der er kun krav om at du løser en af følgende tilvalgsopgaver.

- Administration af beskeder: Det skal være muligt at se og slette bruger beskeder fra Min side.
- Pagination på kommentarer: Der skal laves en pagination på kommentarer med fem kommentarer i hver sektion.
- Glemt password: Brugere skal have mulighed for at få et nyt password hvis de har glemt det gamle.

## Design & opsætning

Det nye website skal opsættes sådan, at det er i overensstemmelse med det udleverede design og kravspecifikation.

Design til sitet er lavet i Figma og du kan finde det under afsnittet Ressourcer. Kunden er dog modtagelig for ændringer i designet, hvis disse kan argumenteres til kundens fordel.

## Webbaseret API

Sitets indhold skal kaldes fra et webbaseret API. Alle data er vedlagt opgaven i form af CSV-filer. Det er din opgave at bygge en database ud fra disse data og sørge for at denne kan fungere som API. Det anbefales at du bruger Supabase til denne del af opgaven.

Du finder CSV data på følgende link: [https://github.com/Webudvikler-TechCollege/Bagtanker-Files/tree/main/CSV](https://github.com/Webudvikler-TechCollege/Bagtanker-Files/tree/main/CSV)

## Rapport

Du skal udarbejde en projektrapport sammen med opgaveløsningen. Projektrapporten skal indeholde følgende:

- Vurdering af din egen indsats og gennemførelse af prøven.
- Argumentation for de valg du har truffet under løsningen af opgaven.
- Redegørelse for oprindelsen af de forskellige kodeelementer i prøven.
- Fremhævelse af eventuelle særlige punkter til bedømmelse.
- Angivelse af URL adresser, brugernavne og passwords der er nødvendige for at lærer og censor kan se opgaven.
- Eventuelle bilag

### Forsiden af rapporten skal indeholde:

- Opgavens navn
- Dit navn og holdnummer
- URL til GitHub repository
- Brugernavn/adgangskoder

Omfanget af rapporten skal være på maksimum fem A4-sider eksklusive bilag. Projektrapporten navngives med dit navn plus rapport og afleveres som en pdf-fil eller en markdown fil i dit Github repository. Eksempel: dit_navn_rapport_bagtanker.pdf.

## Prioritetsliste

Herunder finder du en liste over hvordan du bør prioritere i opgaven:

1. **Opsætning af database:** Start med at opbygge din database ud fra de vedlagte CSV-filer.
2. **Generel opsætning af design:** Sitet skal stå tilnærmelsesvist færdigt i HTML og CSS.
3. **Integration af data og billeder:** Få styr på dine JavaScript fetch af forskellige data og billeder fra API’et.
4. **Kontaktformular:** Formularen skal stå færdig med validering og funktionalitet.
5. **Login:** Det er vigtigt at brugere kan logge ind på sitet – ellers kan de ikke kommentere de forskellige brød opskrifter.
6. **Kommentarer:** Hvis en bruger kan logge ind, skal de også helst kunne oprette, redigere eller slette en kommentar på de forskellige opskrifter.

## Aflevering

Inden fristens udløb skal du aflevere din rapport og filer til dit projekt i et repository på Github. Derefter skal du aflevere et link til dit Github repository som besvarelse til opgaven på Moodle.

**Deadline for aflevering er fredag den 23. august 2024 kl. 14:00.**

God arbejdslyst! 😊
# Affaldsguiden-Files
