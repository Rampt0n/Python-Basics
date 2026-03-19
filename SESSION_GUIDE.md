# Workshop-Leitfaden: Zwei Sessions

## Überblick

| | Session 1 | Session 2 |
|--|-----------|-----------|
| **Thema** | Python & pandas Grundlagen | ETL-Pipeline & Visualisierung |
| **Dauer** | ca. 4 Stunden | ca. 4 Stunden |
| **Voraussetzung** | Keine | Session 1 abgeschlossen |

---

## Session 1 — Python & pandas Grundlagen

### Zeitplan (ca. 4 Stunden)

| Zeit | Inhalt | Notebook |
|------|--------|----------|
| 0:00 – 0:20 | Begrüßung, Umgebung einrichten, Jupyter-Einführung | — |
| 0:20 – 1:50 | Python Grundlagen | `01_Python_Grundlagen.ipynb` |
| 1:50 – 2:05 | **Pause** | |
| 2:05 – 3:45 | pandas Grundlagen | `02_Pandas_Grundlagen.ipynb` |
| 3:45 – 4:00 | Fragen & Ausblick auf Session 2 | — |

### Kerninhalte (Grundlage für Session 2)

- Variablen, Datentypen (`int`, `float`, `str`, `bool`)
- F-Strings
- `if / elif / else`
- Listen und `for`-Schleifen
- Funktionen mit `def` und `return`
- Dictionaries
- `import pandas as pd`, DataFrame erstellen
- Spalten auswählen und filtern
- Einfache Aggregationen (`sum`, `mean`, `groupby`)
- Fehlende Werte erkennen (`isnull`)

### Optionale Inhalte (für schnelle Teilnehmer)

Notebook: **`Session1_Extras.ipynb`**

- List Comprehensions
- Lambda-Funktionen
- `*args` und `**kwargs`
- Erweiterte String-Methoden und Regex-Grundlagen
- Method Chaining in pandas
- `.query()` als Alternative zum Filtern
- Erweiterte Aggregationen mit `.agg()`
- `pd.cut()` und `pd.qcut()` für Kategorisierung

---

## Session 2 — ETL-Pipeline & Visualisierung

### Zeitplan (ca. 4 Stunden)

| Zeit | Inhalt | Notebook |
|------|--------|----------|
| 0:00 – 0:15 | Recap Session 1, Fragen | — |
| 0:15 – 1:00 | Daten Extrahieren (CSV, JSON, API) | `03_ETL_Extract.ipynb` |
| 1:00 – 1:50 | Daten Transformieren | `04_ETL_Transform.ipynb` |
| 1:50 – 2:05 | **Pause** | |
| 2:05 – 2:45 | Daten Laden & vollständige Pipeline | `05_ETL_Load.ipynb` |
| 2:45 – 3:45 | Visualisierung | `06_Visualisierung.ipynb` |
| 3:45 – 4:00 | Abschluss & nächste Schritte | — |

### Kerninhalte

- CSV einlesen (`pd.read_csv`) und exportieren (`to_csv`)
- JSON einlesen
- Typische Datenprobleme bereinigen (Datentypen, fehlende Werte, Duplikate)
- Neue berechnete Spalten
- Ergebnis als CSV oder in SQLite speichern
- Balken- und Liniendiagramm mit matplotlib

### Optionale Inhalte (für schnelle Teilnehmer)

Notebook: **`Session2_Extras.ipynb`**

- Reguläre Ausdrücke (Regex) zur Textbereinigung
- Parquet als effizientes Dateiformat
- Erweiterte SQL-Abfragen (Window Functions, CTEs)
- Interaktive Dashboards mit plotly
- Logging in ETL-Pipelines
- Große Dateien mit `chunksize` verarbeiten

---

## Hinweise für Trainer

### Umgebung einrichten (vor Session 1)
Sicherstellen, dass bei allen Teilnehmern folgendes funktioniert:
```bash
pip install -r requirements.txt
jupyter notebook
```
Am besten als Hausaufgabe vor dem Workshop oder 15 Minuten Puffer einplanen.

### Umgang mit unterschiedlichem Tempo
- Schnelle Teilnehmer: direkt zum jeweiligen Extras-Notebook verweisen
- Langsamere Teilnehmer: Übungen können übersprungen und die Musterlösung gemeinsam besprochen werden
- Die Musterlösungen liegen im Unterordner `Loesungen/` als separate `*_Loesungen.ipynb`-Dateien

### Zwischen den Sessions
Teilnehmer können die Notebooks zuhause wiederholen. Alle Notebooks laufen komplett offline (außer dem optionalen API-Beispiel in Notebook 3, das einen Offline-Fallback enthält).
