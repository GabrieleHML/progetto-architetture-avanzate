# Implementazione dell’algoritmo DBSCAN e sua ottimizzazione mediante istruzioni SIMD

Questo progetto presenta l'implementazione dell'algoritmo di clustering **DBSCAN** e una successiva ottimizzazione della sua performance attraverso l'utilizzo di istruzioni **SIMD** (Single Instruction, Multiple Data).

---

## Descrizione del progetto

Il lavoro si basa sul paper originale "A Density-Based Algorithm for Discovering Clusters in Large Spatial Databases with Noise" di Martin Ester, Hans-Peter Kriegel, Jorg Sander e Xiaowei Xu. Partendo da questa base teorica, io e il mio collega **Giovanni Pascuzzi** abbiamo sviluppato una nostra implementazione dell'algoritmo in linguaggio **C**.

L'obiettivo principale è stato non solo replicare la logica di DBSCAN, ma anche esplorare metodi per migliorarne l'efficienza computazionale. Per questo motivo, abbiamo ottimizzato l'implementazione base sfruttando le istruzioni SIMD, una tecnica che consente di eseguire la stessa operazione su più elementi di dati contemporaneamente, riducendo significativamente i tempi di calcolo.

### Versioni disponibili

Per confrontare le performance e dimostrare l'impatto delle ottimizzazioni, l'algoritmo è disponibile in diverse configurazioni:

- **Versioni a 32 e 64 bit**: Implementazioni ottimizzate per architetture a 32 e 64 bit.
- **Supporto OpenMP**: Per ciascuna delle versioni (32 e 64 bit), è disponibile una variante che utilizza **OpenMP** per la parallelizzazione, permettendo di sfruttare appieno i core multi-thread dei moderni processori.

Una descrizione dettagliata dell'implementazione, delle scelte architetturali e dei risultati dei test di performance è disponibile nella **relazione completa** presente nel repository.

---

## Contesto

Questo progetto è stato realizzato nell'ambito del corso di **ARCHITETTURE AVANZATE DEI SISTEMI DI ELABORAZIONE E PROGRAMMAZIONE** durante l'anno accademico 2023/2024 presso l'**Università della Calabria**.

Desideriamo ringraziare il Prof. **Fabrizio Angiulli** e la Dott.ssa **Simona Nisticò** per la loro supervisione e per averci fornito un template di partenza che ci ha guidato nella strutturazione del progetto.
