# Startkode demonstrasjonsprosjekt

Dette repository er tenkt å demonstrere hvordan startkode distribueres via Git og stegene for å levere inn koden.

## Steg 1: Clone start over på egen GitHub konto

Begynn med å opprette en kopi av denne oppbevaringsplassen ved å bruke *Use this template* (se øverste høyre hjørne på github-websiden). Du vil da få en kopi av oppbevaringsplassen med startkoden på din egen github konto. Du kan nå *clone* denne kopien ned på egen PC (bruk eks. GitHub Desktop).

For gruppeoppgaver er det kun en person i gruppen som skal utføre *Use as template* på startkoden. Den som har utført *Use as template* kan etterfølgende gi tilgang til sin lokale kopi av oppbevaringsplassen til de andre gruppe-medlemmer ved å bruke *Settings* og *Manage Access* på GitHub. De andre gruppemedlemmer kan etterfølgende *klone* oppbevaringsplassen ved å bruke eks. Github Desktop. På denne måten vil alle gruppe-medlemmer jobbe på samme oppbevaringsplass og dele koden som implementeres.

## Steg 2: Importe startkoden og enhetstester inn i IntelliJ

Start-koden ligger i et prosjekt som er organisert slik at bygge-systemet Maven automatisk kan brukes til å kompilere koden og kjøre test i GitHub-skyen.

Importer prosjekt inn i IntelliJ ved å bruke *File* -> *Open* og navigere til mappen der startkoden fra steg 1 er lagret.

Klassene `Grensnitt.java` og `Kalkulator.java` inneholder starten på metodene dere som skal implementeres. Disse finnes under `src/main/java` i prosjektet.

Klassen `TestKalkulator`  inneholder JUnit-enhettester som kan brukes til å teste implementasjon av metodene etterhvert som de implementeres. Disse finner du under `src/test/java` i prosjektet.

Testene kan kjøres ved å åpne filen som inneholder tester og velge *Run* eller ved å trykke på de grønn play-ikoner ved linjenumere.

## Steg 3: Implementere og pushe kode til GitHub

Etterhvert som metodene i oppgavene implementeres kan koden legges opp på GitHub ved å bruke *Commit* etterfulgt av *Push* i GitHub Desktop. Om andre gruppemedlemmer skal ha tilgang til endringer som du har lagt opp, da må de utføre *Fetch* fra deres GitHub Desktop for å oppdatere deres lokale kopi av oppbevaringsplassen.

Om gruppemedlemmer har gjort samtidige endringer på filer og disse endringer er i konflikt med hverandre da må dere gjøre en merge.

Når koden legges opp på GitHub ved å utføre en push vil GitHub sky-tjenesten automatisk kjøre testene og resultatet kan sees ved å gå inn under *Actions* på web-siden for oppbevaringsplassen på GitHub og velge seneste workflow.

## Steg 4: Sjekk at alle metoder fungerer og push til GitHub

Når alle metoder i oppgaven fungerer dvs. alle enhets-test passerer, da må du huske å pushe koden opp på GitHub.

Når koden er pushet opp på GitHub gå inn under *Actions* for oppbevaringsplassen. Sjekk at de automatiske testene som blir kjørt når du legger opp koden har et grønt tick på seg.
