# Salute-e-Benessere-Updates

Applicazione desktop professionale per la gestione delle valutazioni di salute e benessere dei lavoratori.

**Salute e Benessere Aziendale** è progettata per supportare il professionista sanitario nella raccolta dei dati, nell'elaborazione delle valutazioni e nel monitoraggio dell'evoluzione del paziente nel tempo.

## Funzionalità

* 👤 **Gestione dei pazienti**

  * Anagrafica dei pazienti
  * Ricerca e consultazione dei pazienti
  * Storico delle valutazioni

* 📋 **Valutazioni**

  * Creazione di nuove valutazioni
  * Salvataggio delle valutazioni come bozze
  * Completamento e modifica delle valutazioni
  * Confronto tra valutazioni effettuate in momenti diversi

* 📊 **Elaborazione dei dati**

  * Calcolo automatico degli indicatori previsti
  * Gestione di diverse metodologie di valutazione
  * Parametri e formule configurabili
  * Risultati salvati insieme alla valutazione

* 👨‍⚕️ **Profilo del medico**

  * Informazioni professionali
  * Struttura e contatti
  * Logo e firma
  * Gestione delle credenziali di accesso

* 📄 **Report**

  * Generazione di report delle valutazioni
  * Riepilogo dei risultati
  * Confronto con valutazioni precedenti
  * Utilizzo automatico dei dati professionali del medico

* 📤 **Esportazione**

  * Esportazione dei dati e dei report nei formati supportati dall'applicazione

* ⚙️ **Configurazione**

  * Formule configurabili
  * Storico delle modifiche alle formule
  * Parametri modificabili senza modificare il programma

* 🔄 **Aggiornamenti automatici**

  * Controllo della disponibilità di nuove versioni
  * Download dell'aggiornamento direttamente dall'applicazione
  * Verifica crittografica degli aggiornamenti

## Privacy e sicurezza

I dati dei pazienti e delle valutazioni sono gestiti **localmente sul computer** sul quale è installata l'applicazione.

Il database locale contiene i dati necessari al funzionamento dell'applicazione e non viene incluso nel repository del progetto né negli installer distribuiti.

Le credenziali di accesso non vengono memorizzate in chiaro: le password vengono salvate utilizzando un **hash Argon2**.

I dati personali, i database locali, i report e gli eventuali file personali del professionista non vengono inclusi nel codice sorgente o nelle release dell'applicazione.

> **Importante:** l'applicazione tratta dati potenzialmente sensibili. È responsabilità dell'utilizzatore proteggere il computer, l'account del sistema operativo e i backup contenenti i dati.

## Aggiornamenti

L'applicazione dispone di un sistema integrato per il controllo degli aggiornamenti.

Quando viene pubblicata una nuova versione, l'applicazione può:

1. verificare la disponibilità dell'aggiornamento;
2. informare l'utente della nuova versione;
3. scaricare l'aggiornamento;
4. verificarne la firma;
5. installare la nuova versione.

Gli aggiornamenti vengono distribuiti tramite GitHub Releases.

## Tecnologia

L'applicazione è sviluppata utilizzando:

* **Tauri 2** — framework desktop
* **React** — interfaccia utente
* **TypeScript** — sviluppo frontend
* **Rust** — backend e logica applicativa
* **SQLite** — database locale
* **Argon2** — protezione delle password

## Sistemi supportati

Sono previste versioni per:

* 🪟 **Windows**
* 🍎 **macOS**

Gli installer vengono pubblicati nelle release dell'applicazione.

## Struttura del progetto

Il progetto è organizzato principalmente in:

```text
Salute-e-Benessere-aziendale/
├── src/                    # Frontend React
├── src-tauri/              # Backend Rust e configurazione Tauri
│   ├── src/
│   └── tauri.conf.json
├── public/                 # Risorse pubbliche
└── package.json
```

Il database dell'applicazione viene creato nella directory dati locale del sistema e **non viene salvato all'interno del progetto**.

## Versioning

Il progetto utilizza il versionamento semantico.

Esempio:

```text
v0.1.0
v0.1.1
v0.2.0
v1.0.0
```

Le release vengono generate automaticamente tramite **GitHub Actions**.

## Licenza

Questo software è un progetto proprietario.

Il codice sorgente non è destinato alla redistribuzione o alla modifica da parte di soggetti esterni senza autorizzazione del proprietario.
