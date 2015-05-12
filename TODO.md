---
title: "ToDo and dones for Re-submission"
author: "Lutz Göhring"
date: "May 7, 2015"
output: html_document
---
1. ~~LG: berücksichtigt die Probleme dokumentiert auf http://www.stats.ox.ac.uk/pub/bdr/donttest/Old/rriskDistributions.out~~
2. Paket Checks mit R CMD check --as-cran: bis keine weiteren NOTES (und ERRORs oder WARNINGs) produziert werden wir wie folgt checken:
    * LG: dokumentiert die Ergebnisse in Datei cran-comments.md
    1. ~~LG: unter Linux mit R-devel~~
    2. ~~LG: win builder (R-devel und R 3.2.0): dazu kurzzeitige Änderung in DESCRIPTION: maintainer zu Matthias Flor (MF)~~
      * ~~MF: leitet das Ergebnis an LG per e-mail weiter~~
      * ~~LG: in file DESCRIPTION: maintainer zurück auf Matthias Greiner~~
3. Herstellen der Release Version
    1. falls möglich: GitHub Repository: 
        1. ~~MF: organisiert GitHub repository~~
        2. ~~MF: (falls nötig) ermöglicht LG Zutritt dazu~~
        3. ~~MF: richtet master branch ein mit letztem release als head~~
        4. ~~LG: kreiert neuen branch: "re-submission"~~
        5. ~~LG: pushed seine Überarbeitete Version auf branch "re-submission"~~
        6. ~~LG: pull request in master branch~~
        7. ~~MF: bearbeitet pull request und merged in master branch~~
    2. andernfalls:
        1. LG: schickt seine überarbeitete Paket Version (als .tar.gz )an MF
        2. MF: merged mit letztem release
        3. MF: feedback an LG
4. Finale Checks:
    1. MF: checked unter Windows ( R 3.2.0) und win builder (R-devel) und überarbeitet (falls nötig) das Paket bis keine weiteren NOTEs auftauchen. Insbesondere:
        + downstream dependency checks (dies hatte ich beim Telefonat vergessen!)
    2. MF: falls kein Repository: MF schickt das überarbeitete Paket an LG weiter
    3. LG: checked unter Linux (R-devel) und überarbeitet (falls nötig) das Paket bis keine weiteren NOTEs auftauchen
    4. LG: falls kein Repository: leitet das überarbeitete Paket an MF zurück
5. Release:
    * MF: organisiert die re-submission bei CRAN

