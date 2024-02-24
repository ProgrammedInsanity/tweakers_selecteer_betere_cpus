UserScript voor het selecteren van CPU's met een hogere rang bij laptops vergelijken.

Deze UserScript is ontworpen om te werken op de website https://tweakers.net/laptops/vergelijken/*. Het biedt functionaliteit om CPU's met een hogere rang te selecteren en alle CPU's op de pagina te deselecteren.
Het voegt twee knoppen toe, één voor het selecteren van cpu's met een hogere rang dan de huidige geselecteerde. En een knop om alle cpu's te deselecteren.

CPU-ranggegevens zijn afkomstig van (https://www.cpubenchmark.net/cpu_list.php).

Hoe het werkt
Het script decodeert en decomprimeert eerst een base64-string om CPU-gegevens te krijgen. Vervolgens biedt het verschillende functies om met de webpagina te interageren:


searchForCpuSoc(): Zoekt naar de CPU/SOC-sectie op de webpagina.

getSelectedCpus(): Haalt de namen van de momenteel geselecteerde CPU's op.

getCpusWithHigherRank(): Haalt de namen van CPU's op die een hogere rang hebben dan de momenteel geselecteerde CPU's
.
selectCpusWithHigherRank(): Selecteert de CPU's die een hogere rang hebben dan de momenteel geselecteerde CPU's.

unselectAllCpus(): Deselecteert alle CPU's.

addInputButtonToCpusoc(text, onclick): Voegt een knop toe met de opgegeven tekst en onclick-functie aan de CPU/SOC-sectie.

addStyles(css): Voegt de opgegeven CSS toe aan de webpagina.

loadButtons(): Voegt de knoppen 'Selecteer CPU's met een hogere rang' en 'Deselecteer alles' toe aan de CPU/SOC-sectie.

Wanneer de webpagina wordt geladen, wordt de functie loadButtons() aangeroepen om de knoppen aan de pagina toe te voegen.


Hoe te gebruiken
Installeer een UserScript-manager in uw browser, zoals Tampermonkey of Greasemonkey.
Voeg dit script toe aan uw UserScript-manager.
Navigeer naar https://tweakers.net/laptops/vergelijken/*.
Gebruik de knop 'Selecteer CPU's met een hogere rang' om CPU's te selecteren met een hogere rang dan de momenteel geselecteerde CPU's.
Gebruik de knop 'Deselecteer alles' om alle CPU's te deselecteren.
