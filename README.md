# Vinted Photo Studio v2.2 — Studio Light

App web iPhone: https://26ale93-lab.github.io/vinted-photo-studio/

## Novità
- Grafica Studio Light rifinita: intestazione compatta persistente, tipografia, spaziature, anteprima e miniature.
- Editor con sezioni ordinate: **Aspetto del prodotto** e **Sfondo**.
- Dopo aver generato la maschera AI, i preset fotografici sono applicati alla regione del prodotto mentre lo sfondo originale resta separato, poi viene pulito o sostituito. Questo riduce le interferenze tra le due regolazioni.
- Mantiene preset, pannello regolazioni, prima/dopo, pulizia AI, rimozione sfondo, rullino iOS, export foto e ZIP.

## Limitazioni
La separazione è affidabile solo quanto la segmentazione AI: bordi fini e prodotti chiari possono essere classificati male. Senza maschera AI gli stili si applicano all'intera foto. Verificare sempre fedeltà dei colori, loghi, condizioni e difetti del prodotto. La condivisione Safari richiede un'azione dell'utente per salvare nel rullino. Collaudo Safari iPhone da completare.


## v2.2 — salvataggio multiplo nel rullino
Nella sezione «4. Salva le foto» è presente il pulsante **Salva tutte nel rullino**. Prepara le singole immagini elaborate e prova ad aprire il menu di condivisione iOS con tutti i file. Se Safari non supporta la condivisione multipla, offre automaticamente un archivio ZIP. Il salvataggio nell'app Foto richiede una conferma manuale dell'utente. La preparazione asincrona dei file può far perdere l'autorizzazione temporanea del gesto di Safari: funzione da verificare su iPhone reale.


## v2.2 — Restyling premium
Palette blu notte e turchese, fondo grigio perla, contrasti più coerenti, anteprima fotografica e miniature rifinite, pulsanti e controlli iPhone più leggibili, salvataggio multiplo come azione principale. Funzionalità fotografiche invariate. Verificare in Safari su iPhone.


## v2.2 — cambiamento cromatico evidente
Testata blu notte con testo bianco e bordo ciano; sfondo grigio azzurrato; azioni principali turchesi; pulsante salvataggio multiplo con gradiente blu/ciano. Tutti gli strumenti fotografici precedenti invariati.


## v2.2: correzione regolazioni fotografiche
La luminosità, il contrasto, la saturazione e il bilanciamento caldo/freddo sono calcolati direttamente sui pixel (senza dipendere da `CanvasRenderingContext2D.filter`). Il comando Migliora foto ricalcola ora l'ottimizzazione automatica e aggiorna i cursori. Range ampliati per permettere di vedere l'effetto delle regolazioni. Le modifiche sono più evidenti, ma per gli annunci reali mantenere colori e difetti fedeli. Da testare su Safari iPhone.


## v2.2 — Sistema capo (modalità sicura)
Introdotto nel pannello della singola foto **Sistema capo · allineamento sicuro**: rotazione entro ±15° e centratura orizzontale/verticale entro ±12%, con adattamento dell'intera foto nello spazio di destinazione per evitare di tagliare il prodotto. La trasformazione è globale e non altera la geometria relativa di tessuto, loghi, toppe e maniche. Il confronto originale/anteprima mostra le regolazioni provvisorie; **Applica** conferma, **Annulla** ripristina l'ultimo allineamento confermato e **Ripristina** azzera la trasformazione. Le esportazioni usano solo gli allineamenti confermati. La modalità AI sperimentale non è stata implementata: non è stato validato un modello per riordinare la posa senza falsificare i dettagli reali. Funzionalità esistenti mantenute nel codice; test su Safari iPhone e qualità visiva reale ancora necessari.
