# Finance Analysis

This repository contains a Jupyter Notebook used to analyze subscription data and perform basic financial analysis.

## Assunzioni del modello

Per sviluppare l’analisi sono state adottate alcune assunzioni semplificative:

Durata del servizio: si assume che ogni abbonamento abbia una durata fissa di 365 giorni a partire dalla start_date.

Riconoscimento dei ricavi: i ricavi sono riconosciuti secondo il principio di competenza economica, distribuendo il valore fatturato uniformemente lungo i 365 giorni di servizio.

Base per il riconoscimento dei ricavi: il ricavo giornaliero è calcolato utilizzando il fatturato netto (invoice_amount − refund_amount), in modo da escludere gli importi restituiti ai clienti.

Rimborsi: si assume che i rimborsi riducano immediatamente sia il fatturato sia la cassa incassata.

Incassi: la cassa incassata è calcolata come fatturato meno rimborsi, assumendo che le fatture siano pagate nello stesso mese di emissione.

## Files

- `finance_analysis.ipynb` – main notebook containing the analysis
- `subscriptions.csv` – dataset used in the notebook
- `requirements.txt` – Python dependencies required to run the notebook

## Setup

1. Install the required Python packages:

```
pip install -r requirements.txt
```

2. Launch Jupyter:

```
jupyter lab
```

or

```
jupyter notebook
```

3. Open `finance_analysis.ipynb` and run the cells.

## Notes

The notebook reads the dataset `subscriptions.csv`, which must remain in the same folder as the notebook.
