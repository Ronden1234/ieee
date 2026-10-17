# Aggiornamento del sito della conferenza: dalla vecchia edizione alla nuova

Il sito statico (HTML/CSS/JS) della conferenza precedente, preso da una repo GitHub pubblica, viene riadattato per la nuova edizione.
Contenuti, date, relatori, programma e grafica vengono aggiornati usando la presentazione PowerPoint della nuova conferenza e le istruzioni dell'utente.

## Per chi è
- Organizzatori della conferenza che vogliono riusare il vecchio sito senza rifarlo da zero.
- Chi visita il sito: partecipanti, relatori e sponsor, che cercano informazioni aggiornate sulla nuova edizione.

## Funzionalità ed esperienza principali
- **Import della repo**: il sito viene clonato dal link GitHub pubblico e reso visibile in anteprima senza modifiche, così da avere un punto di partenza.
- **Lettura del PPT**: dalla presentazione vengono estratti nome ed edizione dell'evento, date, luogo, tema/claim, relatori (nomi, ruoli, foto se ci sono), programma/agenda, sponsor/partner, contatti, logo e colori.
- **Mappatura vecchio → nuovo**: ogni sezione del sito esistente viene aggiornata con i dati corrispondenti del PPT (hero, about, speaker, programma, location, sponsor, contatti, footer).
- **Sezioni mancanti o superflue**: se il PPT contiene informazioni che il sito non ha, si aggiunge una sezione nello stesso stile; le sezioni della vecchia edizione senza un equivalente nuovo vengono nascoste, non cancellate.
- **Identità visiva**: logo, colori principali e immagini vengono allineati al PPT, mantenendo struttura e layout del sito originale.
- **Modifiche puntuali dell'utente**: dopo il primo aggiornamento si applicano le istruzioni dettagliate scritte dall'utente, una tornata alla volta.
- **Riepilogo delle modifiche**: a ogni tornata, un elenco chiaro di cosa è cambiato e di cosa manca (per esempio dati assenti dal PPT).

## Flusso utente
1. L'utente incolla in chat il link della repo GitHub e carica il file PPT della nuova conferenza.
2. Il sito originale viene messo in anteprima così com'è.
3. Contenuti e grafica vengono aggiornati sulla base del PPT; l'utente vede l'anteprima aggiornata con il riepilogo delle modifiche.
4. L'utente invia le sue modifiche dettagliate; vengono applicate e mostrate in anteprima.
5. Si ripete finché il sito non è approvato, poi i file aggiornati sono pronti da riportare su GitHub o da pubblicare.

## Sensazione UI/UX
- Si mantiene lo stile del sito originale: è un restyling di contenuti, non una riprogettazione.
- I colori e il logo della nuova edizione sostituiscono quelli vecchi in modo coerente in tutte le pagine.
- Il sito resta responsive e leggibile su mobile come l'originale; i problemi evidenti di visualizzazione emersi durante l'aggiornamento vengono corretti.

## Fasi di implementazione
- **Fase 1 – MVP (ora)**: import della repo, anteprima del sito originale, estrazione dei contenuti dal PPT, aggiornamento di tutte le sezioni esistenti (testi, date, relatori, programma, sponsor, contatti, logo e colori), riepilogo delle modifiche e dei dati mancanti.
- **Fase 2**: applicazione delle modifiche dettagliate dell'utente, nuove sezioni o pagine richieste, rifinitura grafica e controllo su mobile.
- **Fase 3**: rifiniture finali (SEO base: titoli e descrizioni, immagine di anteprima per i social, favicon), eventuali piccole funzioni extra richieste (per esempio form di registrazione o link al biglietto) e preparazione per pubblicazione o push su GitHub.

## Assunzioni
- La repo è pubblica e contiene un sito statico HTML/CSS/JS senza backend; il link viene fornito all'inizio del lavoro.
- Il PPT della nuova conferenza viene caricato in chat (.pptx); se arriva in un altro formato (.ppt, PDF) viene convertito prima di estrarne i contenuti.
- Il PPT è la fonte principale per i contenuti; se un dato manca (per esempio indirizzo, prezzi, link di registrazione) resta il segnaposto del vecchio sito, evidenziato nel riepilogo, e non viene inventato.
- Le immagini incluse nel PPT (logo, foto dei relatori, foto della location) vengono riusate sul sito; se mancano si tengono quelle esistenti o un segnaposto neutro.
- Struttura, layout e tecnologia del sito originale restano invariati; nessuna migrazione a un altro framework.
- Le sezioni della vecchia edizione vengono nascoste invece che cancellate, così si possono recuperare.
- La lingua del sito resta quella del sito originale, salvo indicazioni diverse.
- Il sito aggiornato viene consegnato come file modificati pronti per GitHub; la pubblicazione online è un passaggio separato, su richiesta.
