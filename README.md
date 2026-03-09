# Adult Income Classification - Machine Learning Project

## 📋 Descrizione del Progetto

Questo progetto realizza un'analisi completa del dataset **Adult** per la classificazione del reddito (income > $50K) utilizzando tecniche di Machine Learning avanzate.

Il lavoro comprende:
- **Analisi Esplorativa dei Dati (EDA)**: comprensione delle distribuzioni, correlazioni e anomalie
- **Feature Engineering**: creazione e trasformazione delle features
- **Data Splitting e Encoding**: preparazione dei dati per il training
- **Benchmark di Modelli**: confronto di molteplici algoritmi ML
- **Tuning degli Iperparametri**: ottimizzazione delle prestazioni
- **Analisi Diagnostica**: valutazione della calibrazione e affidabilità del modello champion

## 📊 Modelli Implementati

I seguenti modelli sono stati testati e confrontati:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting (XGBoost/LightGBM)

Il modello **XGBoost Tuned** è stato selezionato come modello champion per la sua superiorità in termini di AUC-ROC (0.93+) e stabilità.

## 📁 Struttura del Progetto

```
.
├── adult_notebook.ipynb      # Notebook Jupyter con l'analisi completa
├── adult.pdf                 # Relazione compilata (generato da adult.tex)
├── relazione/                # Sorgenti LaTeX della relazione
│   ├── adult.tex             # File principale LaTeX (gestisce gli appendici)
│   ├── appendice_eda.tex     # Appendice A: Analisi Esplorativa
│   ├── appendice_test_statistici.tex  # Appendice: Test Statistici
│   ├── benchmark.tex         # Appendice: Benchmark dei Modelli
│   ├── data_splitting.tex    # Appendice: Splitting dei Dati
│   ├── encoding.tex          # Appendice: Encoding delle Features
│   ├── feature_engineering.tex # Appendice: Feature Engineering
│   ├── iperparametri.tex     # Appendice: Tuning degli Iperparametri
│   ├── finale.tex            # Appendice: Analisi Approfondita e Calibrazione
│   └── figures/              # Immagini e grafici della relazione
└── README.md                 # Questo file

```

## 🚀 Come Visualizzare i Risultati

### Opzione 1: Visualizzare la Relazione PDF
La relazione completa è disponibile come **`adult.pdf`**. Questo documento è compilato dal file principale `adult.tex` e contiene:
- Introduzione e contesto
- Analisi esplorativa approfondita
- Metodologia di preprocessing
- Risultati comparativi dei modelli
- Analisi diagnostica dettagliata
- Appendici tecniche con risultati estesi
- Conclusioni e raccomandazioni

**Per visualizzare il PDF:**
```bash
# Su Windows
start adult.pdf

# Su Linux/macOS
open adult.pdf
# oppure
xdg-open adult.pdf
```

### Opzione 2: Consultare il Jupyter Notebook
Apri `adult_notebook.ipynb` in Jupyter/VS Code per:
- Esaminare il codice Python completo
- Generare visualizzazioni interattive
- Modificare l'analisi e sperimentare

```bash
jupyter notebook adult_notebook.ipynb
```

### Opzione 3: Leggere i File LaTeX
I sorgenti LaTeX nella cartella `relazione/` contengono la documentazione tecnica strutturata per capitoli.

## 📈 Risultati Principali

- **AUC-ROC del Modello Champion**: > 0.93
- **Accuratezza**: ~85% nel dataset di test
- **Stabilità**: Validazione cross-fold su 5 fold
- **Affidabilità**: Analisi di calibrazione e ranking ability

## 🛠️ Requisiti

Per eseguire il notebook Python sono necessari:
- Python 3.8+
- pandas, numpy, scikit-learn
- xgboost, lightgbm
- matplotlib, seaborn, plotly
- scipy (per test statistici)

## 📝 Licenza

```
Copyright © 2026 Andrea Palazzo
Tutti i diritti riservati (All rights reserved).

Questo software non è concesso in licenza per la distribuzione, 
la modifica o l'uso commerciale senza l'esplicito permesso scritto 
dell'autore.

This software is not licensed for distribution, modification, or 
commercial use without explicit written permission from the author.
```

Per richieste di utilizzo commerciale o permessi speciali, 
contattare direttamente l'autore.

---

**Autore:** Andrea Palazzo  
**Data di Creazione:** 2026
