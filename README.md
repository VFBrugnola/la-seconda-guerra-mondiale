# 🗺️ La Seconda Guerra Mondiale — Mappa Interattiva

Un'applicazione web didattica per esplorare la Seconda Guerra Mondiale attraverso mappe interattive, dati storici e materiali multimediali.

## Funzionalità

- **Mappa principale** con confini del 1939 colorati dinamicamente per schieramento (Asse / Alleati / Neutrali), aggiornati in tempo reale al cambiamento dello slider temporale (es. URSS diventa Alleata nel giugno 1941, Italia nel settembre 1943)
- **Slider temporale** da settembre 1939 ad agosto 1945 (73 mesi), con 7 periodi storici selezionabili (Invasione della Polonia, Guerra Lampo in Occidente, Battaglia d'Inghilterra, Operazione Barbarossa, Svolta di Stalingrado, Liberazione dell'Europa, Guerra nel Pacifico)
- **Linee del fronte animate** per 4 teatri di guerra: Fronte Occidentale, Fronte Orientale, Nord Africa, Fronte Italiano — aggiornate mese per mese
- **Frecce di movimento** per le operazioni principali: invasione della Polonia, Blitzkrieg nelle Ardenne, tre armate di Barbarossa, Operazione Urano, D-Day, Operazione Bagration
- **27 eventi storici** con popup informativi: battaglie, conferenze diplomatiche, stragi, attacchi nucleari
- **Tab Shoah** — mappa dedicata con 15 luoghi della memoria: campi di sterminio (Auschwitz-Birkenau, Treblinka, Belzec…), campi di concentramento, ghetti, siti di fucilazione di massa
- **Tab Armamenti** — 12 armi simbolo con immagini da Wikipedia: Panzer IV, T-34, Tiger I, Spitfire, B-17, U-Boot, USS Enterprise, Katyusha, V-2, Little Boy, Chain Home
- **Tab Perdite** — grafici animati delle vittime militari e civili per le 8 nazioni principali
- **Tab Leader** — biografie e ritratti di Hitler, Churchill, Stalin, Roosevelt, Mussolini, Hirohito, de Gaulle, Rommel

## Come usare

Apri la mappa qui:  
👉 **[vfbrugnola.github.io/la-seconda-guerra-mondiale](https://vfbrugnola.github.io/la-seconda-guerra-mondiale/)**

- Usa lo **slider** in basso per scorrere i mesi del conflitto
- Clicca sui **pulsanti dei periodi** per saltare direttamente a una fase della guerra
- Clicca su uno **stato** sulla mappa per vederne il ruolo nel conflitto
- Clicca su un **evento** (marker colorato) per leggere la descrizione
- Usa i **filtri del fronte** per mostrare o nascondere i singoli teatri di guerra
- Nella tab **Shoah**, clicca sui marker per vedere nome, tipo, vittime stimate e date di attività del sito

## Struttura del progetto

```
la-seconda-guerra-mondiale/
├── index.html              # App completa (UI + logica)
└── data/
    ├── borders_1939.js     # Confini GeoJSON semplificati (base 1938/39)
    ├── periods.js          # 7 periodi storici con date e descrizioni
    ├── nations.js          # 8 nazioni con schieramenti e perdite
    ├── events.js           # 27 eventi georeferenziati
    ├── fronts.js           # 28 linee del fronte per 4 teatri
    ├── movements.js        # 9 operazioni militari con frecce
    ├── shoah.js            # 15 luoghi della memoria
    ├── weapons.js          # 12 armi con schede
    └── leaders.js          # 8 leader con biografie
```

## Tecnologie

- [Leaflet.js](https://leafletjs.com/) v1.9.4 per le mappe interattive
- GeoJSON dei confini storici da [aourednik/historical-basemaps](https://github.com/aourednik/historical-basemaps)
- Immagini dei reperti via [Wikipedia REST API](https://www.mediawiki.org/wiki/API:REST_API)
- Tile ESRI Dark Gray con fallback CartoDB
- File unico HTML + dati separati in JS, nessun framework

## Uso didattico

Progetto realizzato per le classi di storia del Liceo IS Bertrand Russell di Guastalla (RE). Liberamente utilizzabile da altri docenti con citazione dell'autore.

## Licenza

© 2025 Fabrizio Brugnola — [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)  
Libero utilizzo con citazione dell'autore.

> *La Seconda Guerra Mondiale — Mappa Interattiva* — Fabrizio Brugnola, 2025  
> https://vfbrugnola.github.io/la-seconda-guerra-mondiale/
