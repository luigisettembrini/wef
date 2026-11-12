<p align="center"><img src="logo.png" alt="WEF – WhatsApp Export Forensics" width="220"></p>

# WEF – WhatsApp Export Forensics

Programma per Windows che acquisisce e importa le chat esportate da WhatsApp (**iPhone** e **Android**, in qualsiasi lingua), ne estrae messaggi e allegati e produce documenti verificabili a uso forense, con impronte crittografiche e registro delle operazioni.

**[Scarica l'ultima versione](https://github.com/luigisettembrini/wef/releases/latest/download/WEF-win-Setup.exe)** · gratuito, previa attivazione

## Cosa fa

### Acquisizione dal telefono
- **Android**: con il telefono collegato via cavo USB (Debug USB attivo) preleva l'esportazione della chat direttamente dalla memoria del telefono. Calcola le impronte SHA-256 e MD5 sul telefono e di nuovo sul PC e le confronta; legge i dati del dispositivo (modello, numero di serie, versione Android, patch di sicurezza, orologio) e, dalla schermata `*#06#`, IMEI e numero di serie. Non installa nulla sul telefono e non modifica il file.
- **iPhone**: preleva l'esportazione dal backup locale cifrato creato da iTunes o Dispositivi Apple, senza installare nulla sul telefono. Riporta i dati del dispositivo registrati nel backup (modello, iOS, numero di serie, IMEI, numero di telefono), le impronte dei file principali del backup e del file acquisito, e verifica la dimensione e l'integrità dell'archivio.
- Ogni acquisizione produce il **Rapporto di acquisizione** in PDF e il registro dell'acquisizione; la chat può essere importata subito.

### Estrazione e documenti
- **Importazione** di ZIP con allegati o di solo testo, in sola lettura, con impronte MD5 e SHA-256 del file originale, della chat e di ogni allegato.
- Riconoscimento automatico di formato (iPhone o Android), lingua, date e orari; messaggi su più righe e collegamento di ogni messaggio al suo allegato.
- **Excel dei messaggi** con collegamenti agli allegati, **Rapporto di estrazione** e **Report degli allegati** in PDF con miniature.
- **Estrazione parziale**: gli stessi documenti limitati a uno o più periodi, con la numerazione dei messaggi della chat completa.

### Trascrizione dei vocali
- Trascrizione dei messaggi vocali con Whisper, **interamente sul computer**, senza inviare dati all'esterno.
- Di tutta la chat o solo dei **periodi di interesse**; stima del tempo, scelta del modello e della lingua, Excel delle trascrizioni.

### Per la perizia
- **Registro delle operazioni** per ogni estrazione e acquisizione: data, ora, operatore, postazione, versione del programma e impronta di ogni documento generato, a garanzia della catena di custodia.
- **Nota metodologica** pronta da inserire nella relazione: tipi di acquisizione dei dispositivi mobili, metodologia logica adottata, integrità, limiti e riferimenti tecnici e normativi; si copia o si salva in Word.
- **Manuale d'uso** in PDF incluso nel programma.

## Requisiti

- Windows 10 o 11 a 64 bit. Per installare non servono diritti di amministratore.
- **Android**: cavo USB e Debug USB attivo sul telefono; gli strumenti ufficiali di Google (platform-tools) li scarica il programma la prima volta.
- **iPhone**: iTunes o Dispositivi Apple sul PC, per creare il backup cifrato.

## Scarica e installa

**[Scarica l'ultima versione (WEF-win-Setup.exe)](https://github.com/luigisettembrini/wef/releases/latest/download/WEF-win-Setup.exe)**

1. Se il browser segnala che il file "non viene scaricato spesso", scegli *Mantieni* (Edge) o *Conserva comunque* (Chrome).
2. **Prima di avviarlo togli il blocco di Windows**: tasto destro sul file scaricato → *Proprietà* → in basso spunta *Annulla blocco* → *OK*.
3. Avvia il file con un doppio clic: il programma si installa e si apre.
4. Se compare comunque l'avviso di Windows SmartScreen, scegli *Ulteriori informazioni* → *Esegui comunque*.

Le versioni successive vengono proposte dal programma stesso all'avvio e si installano da sole, senza blocchi da togliere. Le novità di ogni versione sono nelle [release](https://github.com/luigisettembrini/wef/releases).

## Licenza d'uso gratuita

L'uso di WEF è concesso gratuitamente, previa attivazione sul computer su cui viene utilizzato. Il codice di attivazione si richiede, gratuitamente, dalla finestra di attivazione del programma: il messaggio viene inviato a **wef@luigisettembrini.it**. Senza attivazione il programma funziona in sola consultazione.

La licenza è personale, non esclusiva e non trasferibile: il programma resta di proprietà esclusiva dell'autore e non può essere ceduto, venduto, modificato o distribuito senza la sua autorizzazione scritta. Il programma è fornito «così com'è», senza garanzie di alcun tipo.

WEF utilizza componenti di terze parti open source, elencati con le rispettive licenze nella finestra *Informazioni* del programma. Android è un marchio di Google LLC; iPhone, iTunes e iCloud sono marchi di Apple Inc.; WhatsApp è un marchio di WhatsApp LLC. WEF non è affiliato a queste società né da esse approvato.

## Contatti

wef@luigisettembrini.it

---
(C) 2023 - 2026 Luigi Settembrini - Tutti i Diritti riservati
