# Vinted Photo Studio per iPhone — v1.5

Web app per correggere fotografie di prodotti e pulire o sostituire lo sfondo prima di caricarle su Vinted.

## Novità v1.5
- Miglioramento automatico adattivo: valuta la luminosità media e usa correzioni più moderate rispetto alla v1.2.
- Pulizia sfondo rapida più prudente: lavora solamente sulle zone classificate come sfondo e protegge i bordi.
- **Pulizia precisa AI**: usa una maschera di segmentazione per evitare di uniformare la superficie del prodotto.
- Intensità pulizia regolabile da 20% a 100%.
- Rimangono prima/dopo, regolazioni manuali, ritaglio, etichette, ordine, download individuale e ZIP.

## Uso su iPhone
Apri https://26ale93-lab.github.io/vinted-photo-studio/ con Safari. Per aggiungere l'app alla schermata Home: Condividi → Aggiungi alla schermata Home.

## Limiti
- La pulizia rapida è euristica e non può distinguere sempre un prodotto chiaro da uno sfondo bianco. La modalità precisa richiede un modello AI scaricato dal browser e può fallire per limiti di memoria/dispositivo.
- Le zone vicine ai bordi non vengono pulite intenzionalmente per ridurre il rischio di alterazioni: possono rimanere aloni che richiedono controllo manuale.
- La correzione fotografica è globale e non garantisce una riproduzione cromatica assoluta. Confrontare sempre gli originali.
- Le foto sono elaborate nel browser; il software non le invia a un backend proprietario. Sono richieste risorse esterne (CDN e modello AI).
- La versione deve essere testata su Safari iPhone con foto reali.


## Novità v1.5 — Salvataggio nel rullino iPhone
Premi **Salva nel rullino** sotto la singola foto. Safari apre il menu di condivisione iOS: scegli **Salva immagine**. Se il menu non è disponibile, compare la fotografia a schermo intero: tieni premuto sull'immagine e scegli **Salva in Foto**. Per motivi di sicurezza del browser, la web app non può scrivere direttamente nel rullino senza l'interazione dell'utente. Rimangono download singolo e ZIP.


## v1.5
Preset rapidi Naturale, Più luminoso, Vinted pulito e Solo sfondo. Pulizia precisa AI tra le azioni principali, pulizia rapida tra gli strumenti secondari. Restano disponibili condivisione nel rullino iOS e download ZIP. Verificare sempre colore, usura e contorni prima della pubblicazione.
