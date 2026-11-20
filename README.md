# Senso Unico Alternato · Alternating One-Way Traffic Simulator

🇬🇧 [English](#english) · 🇮🇹 [Italiano](#italiano)

**▶ Live demo:** https://wizgineer.github.io/senso-unico-alternato/

---

## English

A browser-based simulator for a classic Arduino exercise: a **single-lane bridge** with **two traffic lights**, where traffic from each side must take turns.

Paste an Arduino sketch, press **Run**, and watch what happens: cars arrive, queue, cross the bridge, and sometimes collide head-on if the light cycle doesn't leave enough time to clear the bridge.

### Features

- Runs real Arduino (C++) sketches: `digitalWrite`, `delay`, `millis`, `#define`, constants, functions, arrays, `switch`, `Serial`
- 6 LEDs (red / yellow / green for each side), with automatic pin detection from variable names
- Realistic traffic: safe following distance, gradual start on green, braking before the stop line
- Adjustable traffic density and a share of drivers who **run the red light**
- Collisions are split into *caused by the light cycle* and *caused by red-light runners*
- LED timing diagram, like a logic analyzer
- Repeatable traffic (random seed), so different sketches can be compared fairly
- Single HTML file: works offline, no installation

### Default scenario

- Bridge length: 1 km · Speed limit: 30 km/h
- Default pins: side A → 13 / 12 / 11 · side B → 10 / 9 / 8 (red / yellow / green)
- Faster testing: add `// SCALA 1:10` on the first line to run the timings 10× faster

All values (pins, time scale, traffic, speed) can be changed in the settings panel.

### Good for

- Introductory Arduino and embedded systems courses
- Teaching timing, state sequences and safety margins
- Checking circuits designed in Tinkercad Circuits or on a real board

### Limitations

The sketch is translated to JavaScript, not compiled. `struct`, classes, pointers and `String` methods are not supported. `digitalRead` and `analogRead` do not read real sensors. The user interface is in Italian.

---

## Italiano

Simulatore web per un esercizio classico con Arduino: un **ponte a una sola corsia** con **due semafori**, dove i veicoli dei due lati devono passare a turno.

Si incolla uno sketch Arduino, si preme **Esegui** e si osserva cosa succede: le auto arrivano, fanno la coda, attraversano il ponte e a volte si scontrano, se il ciclo semaforico non lascia il tempo di liberare il ponte.

### Funzioni

- Esegue sketch Arduino (C++): `digitalWrite`, `delay`, `millis`, `#define`, costanti, funzioni, array, `switch`, `Serial`
- 6 LED (rosso / giallo / verde per lato), con riconoscimento automatico dei pin dai nomi delle variabili
- Traffico realistico: distanza di sicurezza, partenza graduale al verde, frenata prima della linea
- Densità del traffico regolabile e una percentuale di automobilisti che **passano col rosso**
- Scontri divisi tra *colpa del ciclo semaforico* e *colpa di chi passa col rosso*
- Cronogramma dei LED, come un analizzatore logico
- Traffico ripetibile (seme casuale), per confrontare codici diversi alle stesse condizioni
- Un solo file HTML: funziona anche offline, senza installare nulla

### Scenario predefinito

- Ponte di 1 km · Limite 30 km/h
- Pin predefiniti: lato A → 13 / 12 / 11 · lato B → 10 / 9 / 8 (rosso / giallo / verde)
- Prove veloci: scrivere `// SCALA 1:10` nella prima riga per accelerare i tempi di 10 volte

Pin, scala dei tempi, traffico e velocità si cambiano dal pannello Impostazioni.

### Adatto a

- Corsi introduttivi di Arduino e sistemi embedded
- Lezioni su tempi, sequenze di stati e margini di sicurezza
- Verificare circuiti progettati in Tinkercad Circuits o su una scheda reale

### Limiti

Lo sketch viene convertito in JavaScript, non compilato. Non sono supportati `struct`, classi, puntatori e i metodi di `String`. `digitalRead` e `analogRead` non leggono sensori reali.

---

## Credits

Created by **Wizgineer**. Developed with the assistance of Claude (Anthropic). Independent project, not affiliated with or endorsed by Anthropic.

Sviluppato con l'assistenza di Claude (Anthropic). Progetto indipendente, non affiliato né approvato da Anthropic.

## License

[MIT](LICENSE): free to use, modify and share, with attribution. · Libero di usarlo, modificarlo e condividerlo, citando l'autore.
