# A cosa risponde ciascuna pagina

Appunti di lavoro sulla struttura del sito. Non viene pubblicato.

Il criterio: ogni pagina deve rispondere a **una domanda sola**. Se due pagine
rispondono alla stessa, una delle due va ripensata, è il problema che abbiamo
incontrato fra la home e *Cosa facciamo*.

---

## Le pagine che esistono

| Pagina | Domanda a cui risponde | Chi la legge |
|---|---|---|
| **Home** | «Sono nel posto giusto? E dove devo andare?» | tutti, per pochi secondi |
| **Chi siamo** | «Di chi mi sto fidando?» | istituzioni, giornalisti, curiosi |
| **Cosa facciamo** | «Quale delle vostre attività riguarda me?» | chi ha già capito chi siete |
| **Ricerca ed esercitazioni** | «Come fa un cane a trovare una persona?» | curiosi, e chi frequenta il campo |
| **Educazione di base** | «Posso venire col mio cane? Come funziona?» | privati con un cane |
| **Nelle scuole** | «Posso organizzarlo per la mia classe?» | insegnanti e dirigenti |
| **Contatti** | «Come vi raggiungo?» | tutti, quando hanno deciso |

## Le pagine da fare

| Pagina | Domanda a cui risponde |
|---|---|
| **Le persone del gruppo** | «Chi troverò quando arrivo? A chi mi rivolgo?» |
| **Attività** (i post) | «Siete vivi? Cosa avete fatto di recente?» |
| **Sostienici** | «Come posso aiutarvi senza entrare nel gruppo?» |
| **Spiedo** (temporanea) | «Quando è, quanto costa, come prenoto?» |

---

## Come funzionano i post

Ogni notizia, evento o articolo di giornale è **un file** dentro `_posts/`.
La pagina `/attivita/` non contiene link scritti a mano: elenca da sola tutti i
file che trova, dal più recente al più vecchio. Si aggiunge un file, l'elenco si
aggiorna.

**Il nome del file** deve seguire il formato `AAAA-MM-GG-titolo.md`, con la data
di *pubblicazione*. È obbligatorio: senza data Jekyll non lo riconosce come post.

**L'indirizzo della pagina** è invece una scelta nostra, e si scrive nella riga
`permalink:` del post. La convenzione adottata è:

```
/attivita/evento-posto-anno-mese/
```

per esempio `/attivita/dimostrazione-piazza-verolanuova-2026-09/`.

Quattro pezzi, sempre in quest'ordine: **che cosa** è (dimostrazione,
esercitazione, spiedo, incontro), **dove** si è svolto, **in che anno** e **in
che mese**. Il mese a due cifre, così due iniziative dello stesso tipo nello
stesso posto e nello stesso anno non si pestano i piedi.

Perché il posto e l'anno: le iniziative si ripetono, e la stessa cosa si fa in
paesi diversi. Senza quei due pezzi la dimostrazione del 2027, o quella in un
altro Comune, non potrebbe avere un indirizzo suo. Così ogni edizione resta
consultabile e si capisce di cosa si tratta già dall'indirizzo.

Da ricordare: **posto, anno e mese vanno scritti a mano** ogni volta che si crea un
post. Se ci si dimentica il sito funziona lo stesso, ma prima o poi ci si trova
con un conflitto da risolvere.

**L'indirizzo va deciso prima di condividere il link.** Una volta che il link
gira su WhatsApp e nelle chat del paese, cambiarlo significa lasciare un 404 a
chiunque abbia ricevuto il messaggio vecchio, e nessuno scriverà per segnalarlo.
Finché il post è appena creato si cambia liberamente; dopo la prima condivisione,
non si tocca più.

## Dove vanno le immagini

```
assets/images/
├── favicon.png      l'icona del sito, non è un'immagine di contenuto
├── logo/            lo stemma e le sue versioni
├── pagine/          i banner (hero) delle pagine fisse
├── attivita/        i materiali dei post, una cartella per evento
│   └── 2026-09-dimostrazione-verolanuova/
│         locandina.jpg
└── generali/        foto riutilizzabili: cani, campo, esercitazioni
```

Il criterio è **per destinazione, non per tipo**: ogni immagine sta dove sta il
contenuto che la usa. Quando un evento è passato si sa cosa si può archiviare, e
quando si rifà una pagina si sa quali file toccare.

**Una cartella per evento** dentro `attivita/`, con lo stesso schema dei
permalink: `anno-mese-evento-posto`. Così l'ordine alfabetico è anche quello
cronologico, e locandina, foto e ritagli di giornale di quell'evento stanno
insieme invece di finire sparsi.

**`generali/`** è per le foto che si riusano in più punti: un buon primo piano di
un cane al lavoro può stare nella pagina Ricerca oggi e in un post fra sei mesi.
Meglio una copia sola.

### Nomi dei file

Tutto **minuscolo**, **niente spazi**, **niente accenti**, trattini al posto
degli spazi. Non è pignoleria: negli indirizzi web gli spazi diventano `%20` e
gli accenti su alcuni server si rompono.

Sì: `locandina.jpg`, `cane-macerie-01.jpg`
No: `Locandina Definitiva (2).jpg`, `IMG_4471.JPG`

## La home

Il nodo aperto. La difficoltà è che deve fare **due cose insieme**:

1. dire chi siamo, in tre righe, a chi non ci conosce;
2. smistare le persone verso la pagina che riguarda loro.

L'idea dello smistamento per lettore, *sei un privato? sei una scuola? sei un
Comune?*, funziona, e va tenuta. Il rischio è la sovrapposizione con *Cosa
facciamo*: si evita se le due pagine usano **criteri diversi**.

- la home smista per **chi sei** (privato, insegnante, ente, curioso);
- *Cosa facciamo* organizza per **attività** (ricerca, educazione, scuole).

Manca una categoria che oggi non è coperta da nessuna parte: **il Comune o
l'associazione che vuole invitarci a una manifestazione**. Non è educazione di
base, non è scuola, non è ricerca: è una dimostrazione pubblica. Va deciso se
diventa una quarta voce dello smistamento e, in prospettiva, una pagina sua.

Ordine ipotizzato per la home:

1. fascia di apertura con nome, una riga di identità, e la fotografia;
2. avviso temporaneo, quando c'è (spiedo);
3. lo smistamento per lettore, in riquadri;
4. il 112, breve e visibile;
5. le ultime attività, richiamate dai post;
6. l'invito a passare al campo.

## Lo spiedo

In home va il **richiamo**: locandina, data, una riga di informazioni, e il link
al post. I dettagli, menù, prezzi, prenotazioni, «posti esauriti», stanno solo
nel post, così si aggiornano in un punto solo.

Il tema ha una fascia d'avviso che si accende e si spegne da `_config.yml`: è
fatta per questo, e a evento finito basta togliere una riga.
