# Informazioni da raccogliere

Elenco di quello che manca per completare il sito. Ogni voce dice **a chi
chiedere** e **dove finirà** nel sito.

Questo file non viene pubblicato: è escluso dalla costruzione del sito
in `_config.yml`.

---

## Urgente, serve per Chi siamo

- [x] ~~Inquadramento nella Protezione Civile~~ → confermato: **gruppo comunale**,
      scritto in *Chi siamo*.
- [ ] **Numeri del gruppo:** quanti volontari, quante unità cinofile, quanti cani
      operativi, quanti in addestramento. → *Chi siamo*, sezione "Il gruppo oggi"
      (ancora da scrivere).
- [ ] **Statuto in PDF.** Esiste ma non è nelle nostre mani. → da mettere in
      `assets/documenti/` e collegare in fondo a *Chi siamo*.
- [ ] **Iscrizione al RUNTS:** numero di repertorio e data. → *Chi siamo*, tabella
      dei dati.

## Per le pagine successive

- [ ] **Numero di telefono pubblicabile?** Sulla pagina *Educazione di base* c'è
      solo mail e social. Chi vuole sapere se sabato ci siete non scrive una
      mail. Serve un recapito del gruppo, non il cellulare personale di
      qualcuno, a meno che quella persona sia d'accordo.
- [ ] **Come descrivere chi tiene gli incontri**, ora che il gruppo non ha più le
      qualifiche UCIS. Per ora la pagina non parla di istruttori: meglio il
      silenzio di un'imprecisione su titoli e qualifiche.
- [ ] **Inquadramento della parte economica** dell'educazione di base: quota
      associativa, rimborso spese o corrispettivo? Da chiarire anche a livello
      fiscale, visto che si tratta di attività verso non soci. Finché non è
      chiaro, la pagina rimanda a un contatto diretto.
- [ ] **Provare dal telefono il link alle mappe del campo.** Ora cerca il posto
      per nome, "Campo addestramento cinofilo GCV". Se Maps non lo trova o apre
      il punto sbagliato, servono le coordinate del cancello: tenere premuto sul
      punto giusto in Google Maps, copiare i due numeri e sostituirli nei link
      in `contatti.md` e `chi-siamo.md`.
- [ ] **Giorni e orari di ritrovo al campo.** È il dato più utile per chi vuole
      venire a conoscerci. → pagina *Vieni a trovarci*.
- [ ] **Incontri nelle scuole, due dati pratici che mancano:** l'incontro è
      gratuito? (va detto esplicitamente: un dirigente che valuta un'attività ha
      bisogno di saperlo) e con quanto anticipo va richiesto?

## Pagina Ricerca ed esercitazioni

- [ ] **Rileggere il blocco "Come si svolge una ricerca".** È ricostruito, non è
      il vostro protocollo: chi attiva le squadre, con che tempi di uscita, chi
      assegna i settori. Da correggere con chi conosce il regolamento di
      protezione civile.
- [x] ~~Nome esatto delle tecniche di ricerca~~ → è la ricerca in superficie
      (*a scovo*, in tedesco *Flächensuche*). Sul sito è descritta a parole,
      senza nominare tecniche né collegare Wikipedia: scelta voluta.
- [x] ~~Affiliazione IRO/FCI~~ → no: IRO è un brevetto di alto livello che il
      gruppo non ha. La pagina non cita enti né certificazioni, e non deve.
- [ ] **Campo macerie di Ghedi:** link al loro sito e ai loro social.
- [ ] **Nomi degli esami** e dell'ente che li rilascia oggi, dopo l'uscita da
      UCIS. Ora la pagina dice solo "esami".
- [ ] **Due o tre esercitazioni concrete:** dove, quando, con chi. Sono quello
      che rende credibile tutto il paragrafo sulle esercitazioni.
- [ ] **Quante unità operative siamo.** Per ora l'argomento è evitato: meglio
      tacere che dare un numero sbagliato.

## Presenza su Google

- [ ] **Rivendicare la scheda del campo su Google Maps.** Finché non è
      rivendicata, chiunque può proporre modifiche a nome, posizione e orari
      senza chiedercelo. Rivendicandola decidiamo noi: segnaposto corretto,
      orari, foto, link al sito. Da fare da un account Google del gruppo, non
      personale. La verifica arriva di solito con una cartolina: meglio usare
      la sede di Via Marconi 28 che il campo. Da valutare prima in gruppo,
      perché apre anche alle recensioni pubbliche, che non si possono
      disattivare.

## Materiali

- [ ] **Fotografie** del gruppo, dei cani al lavoro, delle esercitazioni.
      Attenzione alle **liberatorie**, soprattutto per le foto scattate nelle
      scuole: senza consenso dei genitori, niente volti di minori.

      Serviranno anche come **banner in cima alle pagine**, al posto della fascia
      verde: una riga `hero_image:` nel front matter e la fascia diventa la
      fotografia. Si può fare una pagina alla volta, man mano che le foto
      arrivano; quelle senza restano verdi.

      Cosa chiedere a chi scatta:
      - **larghe almeno 1600 pixel**, meglio 2000. Il banner occupa tutta la
        larghezza dello schermo e una foto piccola viene sgranata.
      - **soggetto spostato da un lato.** Il centro viene coperto da titolo e
        sottotitolo, e i bordi vengono tagliati sugli schermi stretti.
      - **orizzontali**, non verticali.

      Due cose da fare al momento di metterle sul sito:
      - **ridimensionare e comprimere.** Una foto dal telefono pesa anche 5 MB e
        rallenta il sito su rete mobile: si scende sotto i 300 KB senza
        differenze visibili.
      - aggiungere anche `hero_darken: true`, che stende un velo scuro
        sull'immagine. Il titolo è bianco e su una foto chiara sparirebbe.
- [ ] **Rassegna stampa:** link agli articoli di giornale che vi hanno citato.
      → sezione *Attività*.
- [ ] **Loghi** di eventuali sponsor, convenzioni o patrocini del Comune.
- [ ] **Versione semplificata dello stemma** per gli usi molto piccoli (favicon):
      a 16 pixel lo stemma completo diventa una macchia verde.
- [ ] **Togliere lo sfondo bianco dallo stemma vettoriale.** In
      `assets/images/logo/gcv-vettoriale.svg` il quadrato dietro al cerchio è
      bianco pieno: si vedono quattro angoli bianchi appena il logo finisce su
      un fondo colorato (navbar, hero, footer). Serve renderlo trasparente
      lasciando bianche solo le zone interne al disegno: i musi dei cani e il
      viso. Da fare in Inkscape sul tracciato bianco, oppure ritracciando.

## Dimostrazione del 13 settembre 2026

Il post è già online: `_posts/2026-08-10-dimostrazione-piazza-verolanuova.md`. Dentro al
file ci sono le istruzioni per ogni punto.

- [ ] **CONFERMARE GIORNO E DATA.** Il messaggio sul gruppo diceva "13 settembre"
      senza giorno della settimana: il 13 settembre 2026 è una **domenica**. Se
      l'intenzione era un sabato, la data giusta sarebbe il 12. Da chiarire prima
      di diffondere il link.
- [ ] **Orario** di inizio e fine, anche approssimativo. Ora il post non lo dice.
- [ ] **Cosa si farà nella dimostrazione.** Il testo resta sul generico finché il
      programma non è deciso.
- [ ] **Patrocinio o manifestazione più grande?** Se siamo dentro un evento del
      Comune va detto.
- [ ] **Locandina.** File in `assets/images/`, poi una riga `image:` nel post: da
      sola mette la locandina nella scheda dell'elenco e nelle anteprime di
      WhatsApp e Facebook. Chi la disegna tenga le informazioni al centro, perché
      le anteprime tagliano ai lati.
- [ ] **A evento concluso:** togliere l'avviso dalla home commentando il blocco
      `avviso:` in `_config.yml`. Il post resta nell'archivio.

## Raccolta fondi

- [ ] **5×1000:** testo di presentazione. Il codice fiscale è 97007140177.
- [ ] **Spiedo annuale:** data, luogo, menù, prezzi, come si prenota e entro
      quando. Servirà solo nel periodo dell'evento, la pagina si accende e si
      spegne da `_config.yml`.

## Dominio e accessi

- [ ] **Enforce HTTPS** su GitHub: Settings → Pages. Va spuntato appena GitHub
      finisce di emettere il certificato.
- [ ] **Credenziali del pannello DNS** del dominio, da recuperare e conservare.
