# AlphaLab-Organ
Prototipo sperimentale di Organo/String con generazione del suono a divisori cmos

Studio di una architettura di base adatta a testare le funzionalità di un Organo (o String Machine), realizzato con circuiteria classica degli anni '70.

## Architettura classica:

1. Top octave generator (realizzato con microcontrollore per la gestione del pilotaggio Midi)
2. Divisori Cmos (per la generazione di 8 ottave partendo delle 12 frequenze di clock relative alle note)
3. Routing e mixing delle varie frequenze generate dai divisori
4. Sezione Filtri per la caratterizzazione dei suoni (comuni a tutte le note in caso di Organo classico e per singola nota in caso di String) 

### Ipotesi 1: 
Progettare un hardware di test comprensivo della circuiteria per: 
1. Ricezione dati da interfaccia keyboard (tramite comunicazione seriale Midi TTL)
2. Generazione delle 12 frequenze
3. Divisori cmos per 8 ottave
4. Routing delle varie frequenze generate
5. 12 connettori per moduli di filtraggio 
