# Netflix Originals Analysis (Python/Pandas)

## Obiettivo
Analizzare trend e pattern dei contenuti Netflix: crescita per anno, generi dominanti, paesi, e insight utili.

## Dataset
- Fonte: (https://www.kaggle.com/datasets/shivamb/netflix-shows)
- Campi principali: title, date_added, country, listed_in (generi), type
- Nota: dataset completo incluso `data/netflix_titles.csv`. Istruzioni sotto per riprodurre.

## Metodi / Stack
- Python (Pandas, Matplotlib/Seaborn)
- Passi: cleaning → feature engineering → EDA → visualizzazioni → insight

## Struttura repo
- `notebooks/netflix.ipynb` – analisi completa con grafici
- `data/netflix_titles.csv` – campione dati
- `graphs/` – immagini principali
- `requirements.txt` – dipendenze

## Riproduzione
```bash
python -m venv venv
# Windows: venv\Scripts\activate
# macOS/Linux: source venv/bin/activate
pip install -r requirements.txt
jupyter notebook notebooks/netflix.ipynb
