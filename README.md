# Analisi Idrologica delle Precipitazioni Massime - Stazione di Romeno

Questo repository contiene l'analisi statistica delle serie storiche di precipitazione registrate presso la stazione pluviometrica di *Romeno*. L'obiettivo è la caratterizzazione degli eventi estremi e la definizione delle Curve di Possibilità Pluviometrica (CPP).

---

## 📊 Sintesi dell'Analisi
Il progetto elabora i massimi di precipitazione per diverse durate temporali (*1h, 3h, 6h, 12h, 24h*) utilizzando Python e librerie scientifiche (⁠ pandas ⁠, ⁠ scipy ⁠, ⁠ matplotlib ⁠).

### Punti chiave:
1.  *Analisi Esplorativa: Identificazione di eventi storici eccezionali (es. **56.6 mm in 1h* nel 1986).
2.  *Modellistica Statistica: Fitting delle distribuzioni di probabilità di **Gumbel* (EVD tipo I) e *GEV* (Generalized Extreme Value).
3.  *Validazione: Confronto tramite Q-Q Plot e calcolo dell'errore quadratico medio (RMSE*).
4.  *Progettazione: Calcolo delle altezze di pioggia per tempi di ritorno fino a **100 anni* e stima dei parametri $a$ e $n$ della legge di potenza $h = a \cdot t^n$.

---

## 📂 Struttura del Repository
*   ⁠ romeno_pluvio.ipynb ⁠: Notebook Jupyter con l'intero codice Python dell'analisi.
*   ⁠ Romeno_data.csv ⁠: Dataset originale con le serie storiche.
*   ⁠ elaborati/ ⁠: Cartella contenente i grafici generati (Andamento storico, Boxplot, LSPP, CPP).

---

## 📈 Risultati Principali
Dall'analisi è emerso che:
*   Per le durate brevi (1h-6h), la distribuzione *GEV* mostra un adattamento superiore (RMSE inferiore).
*   Per la progettazione finale (CPP), è stata adottata la distribuzione di *Gumbel* per il principio di parsimonia.
*   L'esponente idrologico $n$ calcolato per la stazione di Romeno è risultato pari a circa *0.41*, indicando una crescita regolare delle altezze di pioggia al variare della durata.

---

## 🛠️ Strumenti Utilizzati
*   *Linguaggio*: Python 3
*   *Librerie*: ⁠ numpy ⁠, ⁠ pandas ⁠, ⁠ scipy.stats ⁠, ⁠ matplotlib ⁠
*   *Ambiente*: Jupyter Lab / Notebook

---

	⁠Analisi caricata il 25/04/2026
