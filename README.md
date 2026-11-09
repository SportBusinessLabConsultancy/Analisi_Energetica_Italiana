# ⚡ Analisi Energetica Italiana

Mappa interattiva multilivello sviluppata in Python con Kepler.gl per l'analisi integrata delle dinamiche energetiche, infrastrutturali, ambientali e di rischio naturale sull'intero territorio italiano.

---

## 📌 Descrizione

Il progetto sviluppa una mappa interattiva multilivello finalizzata all'analisi integrata delle dinamiche energetiche, infrastrutturali, ambientali e di rischio naturale sull'intero territorio italiano. Attraverso l'integrazione di numerosi layer tematici, la mappa consente di esplorare in modo sinottico la relazione tra produzione energetica da fonti rinnovabili, consumi elettrici a scala comunale, disponibilità territoriale per nuove installazioni, vincoli ambientali e caratteristiche di pericolosità sismica.

La mappa interattiva rappresenta uno strumento esplorativo avanzato, in grado di supportare valutazioni territoriali complesse attraverso la sovrapposizione dinamica di layer eterogenei. In questo modo è possibile analizzare la coerenza spaziale tra domanda e offerta energetica, individuare potenziali aree di sviluppo per le fonti rinnovabili, valutare il ruolo delle infrastrutture di rete elettrica e considerare simultaneamente i principali vincoli ambientali e di rischio.

> ⚠️ La mappa interattiva finale (file HTML, 359 MB) supera i limiti di dimensione per il caricamento su GitHub. Per visualizzarla, è necessario eseguire lo script Python in locale.

---

## 🎯 Obiettivi

- Integrare in un'unica piattaforma interattiva multilivello dati energetici, infrastrutturali, ambientali e di rischio naturale relativi all'intero territorio italiano
- Analizzare la distribuzione territoriale delle fonti energetiche rinnovabili e la loro relazione con i consumi elettrici a scala comunale e regionale
- Individuare aree potenzialmente idonee allo sviluppo di nuovi impianti rinnovabili, tenendo conto dei vincoli ambientali, dell'uso del suolo e delle infrastrutture di rete esistenti
- Valutare la coerenza spaziale tra domanda e offerta energetica per decisioni a scala nazionale e macro-regionale

---

## 🔬 Metodologia

**Integrazione e armonizzazione dei dati**
La metodologia si basa su un processo strutturato di integrazione, armonizzazione e visualizzazione di dati geospaziali eterogenei, realizzato interamente in Python. I dataset comprendono informazioni a scala comunale e regionale relative a produzione energetica da fonti rinnovabili (eolico, fotovoltaico, bioenergie, idroelettrico), consumi elettrici, infrastrutture della rete elettrica, uso e copertura del suolo, aree protette, confini amministrativi e classificazione del rischio sismico. Tutti i layer sono stati trasformati in un sistema di riferimento geografico comune per garantire coerenza spaziale.

**Pulizia e semplificazione geometrica**
Una fase centrale del workflow ha riguardato la pulizia e la semplificazione geometrica dei dati tramite GeoPandas. Le geometrie sono state proiettate in coordinate metriche (EPSG:3857) per applicare operazioni di bufferizzazione e semplificazione topologicamente coerente, con tolleranze differenziate in funzione della complessità dei singoli layer. Questo ha permesso di ridurre significativamente il peso dei file mantenendo l'integrità spaziale. I layer finali sono stati esportati in formato GeoJSON ottimizzato.

**Costruzione della mappa**
Tutti i dataset elaborati sono stati caricati in un'unica mappa interattiva realizzata con Kepler.gl, che consente la gestione simultanea di numerosi layer tematici sull'intero territorio nazionale. L'approccio multilivello permette di attivare, disattivare e combinare dinamicamente le informazioni, facilitando l'analisi delle relazioni spaziali tra produzione energetica, consumi, infrastrutture di rete, vincoli ambientali e fattori di rischio.

---

## 📊 Risultati principali

- Realizzata una mappa interattiva nazionale in Kepler.gl con visualizzazione simultanea e dinamica di numerosi layer tematici geospaziali
- Evidenziate forti differenze territoriali tra produzione energetica da fonti rinnovabili, livelli di consumo elettrico e grado di autosufficienza energetica a scala comunale
- Individuate aree con elevato potenziale di sviluppo per eolico e fotovoltaico, nonché zone soggette a vincoli ambientali o a rischio naturale rilevante
- Prodotto uno strumento operativo per analisi esplorative, supporto alle decisioni e pianificazione energetica e territoriale su scala nazionale e macro-regionale

---

## 🛠️ Tecnologie utilizzate

- **Python / Jupyter Notebook** — elaborazione dati e generazione della mappa
- **Kepler.gl** — mappa interattiva multilivello
- **GeoPandas** — caricamento, pulizia e semplificazione geometrica dei dati geospaziali
- **Shapefile / GeoJSON** — formati dati energetici e territoriali

---

## 📁 Struttura del progetto

```
Analisi_Energetica_Italiana/
├── README.md
└── analisi_energetica_italiana_script.ipynb
```

> ⚠️ I dati di input (shapefile energetici e territoriali) e la mappa HTML finale non sono inclusi nel repository per ragioni di dimensione. Le fonti sono indicate nella sezione Dati.

---

## 📂 Dati

| Fonte | Descrizione |
|-------|-------------|
| [Terna](https://www.terna.it) | Rete di trasmissione nazionale, cabine primarie, infrastrutture elettriche |
| [GSE](https://www.gse.it) | Impianti da fonti rinnovabili (eolico, fotovoltaico, idroelettrico, bioenergie) |
| [ISTAT](https://www.istat.it) | Confini comunali e regionali, dati di consumo elettrico |
| [MASE / EUSP](https://www.mase.gov.it) | Aree idonee allo sviluppo di impianti rinnovabili |
| [CORINE Land Cover](https://land.copernicus.eu) | Uso e copertura del suolo |
| [INGV / DPC](https://www.protezionecivile.gov.it) | Classificazione sismica del territorio italiano |

---

## 🔗 Link utili

- 🌐 [Sport Business Lab Consultancy](https://www.sblconsultancy.it/)
