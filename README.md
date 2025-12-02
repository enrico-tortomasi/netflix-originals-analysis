# Netflix Originals Analysis (Python/Pandas)
![Completed](https://img.shields.io/badge/Completed-✓-3CB371)

Analisi esplorativa dei titoli Netflix (film e serie) con l’obiettivo di capire
come si distribuiscono i contenuti nel tempo, per paese e per genere.

Il progetto è pensato per mostrare competenze di base/intermedie in:
pulizia dati con Pandas, analisi esplorativa (EDA) e visualizzazioni semplici.

---

## Dataset
- Fonte: [Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- Campi principali: title, date_added, country, listed_in (generi), type
- Nota: dataset completo incluso `data/netflix_titles.csv`. Istruzioni sotto per riprodurre.

---

## Obiettivi dell’analisi

- Capire come è cambiato nel tempo il numero di contenuti rilasciati.
- Analizzare la distribuzione dei contenuti per paese.
- Analizzare la distribuzione per genere / categoria.
- Mettere in evidenza eventuali pattern (es. focus crescente sulle serie TV).

---

## Strumenti utilizzati

- Python 3.x
- Librerie: `pandas`, `matplotlib`, `seaborn`
- Jupyter Notebook

---

## Workflow

1. Caricamento del dataset (`read_csv`).
2. Pulizia dati:
   - gestione dei valori nulli
   - normalizzazione di date e paesi
   - creazione di colonne derivate (es. anno di rilascio).
3. Analisi esplorativa:
   - conteggi per anno
   - conteggi per paese
   - conteggi per genere / categoria
4. Visualizzazioni:
   - bar chart per numero di titoli per anno
   - bar chart per top paesi
   - grafici per tipo di contenuto (Film vs TV Show).

---

## Struttura del repository

```
netflix-originals-analysis/
│
├─ data/
│   └─ netflix_titles.csv
│
├─ graphs/
│   ├─ (Barplot)Categorie_Ultimi_5_Anni.png
│   ├─ (Barplot)Contenuti_per_anno.png
│   ├─ (Barplot)Regioni_maggior_numero_films.png
│   ├─ (Barplot)Regioni_maggior_numero_serietv.png
│   ├─ (Piechart)Rating_Movies.png
│   └─ (Piechart)Rating_SerieTV.png
│
├─ notebooks/
│   └─ netflix_originals_analysis.ipynb
│
└─ README.md
```

---

## Insight principali

- ## Crescita dei contenuti: la libreria di Netflix Originals è cresciuta significativamente nel tempo, con un aumento annuale dei titoli prodotti.

![1](graphs/(Barplot)Contenuti_per_anno.png)

---

- ### Distribuzione per genere: i generi più comuni sono Drama, Comedy e Action, riflettendo le preferenze degli spettatori.

![2](graphs/(Barplot)Categorie_Ultimi_5_Anni.png)

---
 
- ### Fra i Films presenti sono quelli con rating TV-14 (adolescenti) e TV-MA (publico per adulti) ad occupare più della metà del catalogo disponibile.

![3](graphs/(Piechart)Rating_Movies.png)

---

## Riproduzione

```
bash
python -m venv venv
# Windows: venv\Scripts\activate
# macOS/Linux: source venv/bin/activate
pip install -r requirements.txt
jupyter notebook notebooks/netflix.ipynb
```

---

## Come eseguire il notebook

Clonare il repository.

Installare le dipendenze minimo (pandas, matplotlib, seaborn).

Aprire il notebook in Jupyter / VS Code.

Eseguire tutte le celle in ordine.
