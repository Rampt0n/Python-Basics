# Python Workshop: Grundlagen bis ETL-Pipeline

Eine Notebook-Reihe für Einsteiger ohne Programmiervorkenntnisse. Ziel ist es, die grundlegenden Schritte einer ETL-Pipeline (Extract, Transform, Load) in Python selbstständig umzusetzen sowie Daten zu visualisieren.

## Workshop-Struktur

Der Workshop ist in zwei Sessions à ca. 4 Stunden aufgeteilt. Den detaillierten Zeitplan und Hinweise für Trainer enthält [`SESSION_GUIDE.md`](SESSION_GUIDE.md).

### Session 1 - Python & pandas Grundlagen

| Notebook | Thema |
|----------|-------|
| `01_Python_Grundlagen.ipynb` | Variablen, Datentypen, Bedingungen, Schleifen, Funktionen, Dictionaries |
| `02_Pandas_Grundlagen.ipynb` | DataFrames, filtern, aggregieren, zusammenführen |
| `Session1_Extras.ipynb` | **Optional:** List Comprehensions, `dict.get()`, try/except, String-Methoden, Method Chaining, `.query()`, erweitertes `.agg()`, `pd.cut()`/`pd.qcut()` |

### Session 2 - ETL-Pipeline & Visualisierung

| Notebook | Thema |
|----------|-------|
| `03_ETL_Extract.ipynb` | CSV, Excel, JSON, REST-APIs einlesen |
| `04_ETL_Transform.ipynb` | Bereinigen, Typen korrigieren, Duplikate, Anreicherung |
| `05_ETL_Load.ipynb` | Exportieren (CSV/Excel/SQLite), vollständige Pipeline |
| `06_Visualisierung.ipynb` | matplotlib, seaborn, plotly |
| `Session2_Extras.ipynb` | **Optional:** Parquet, Window Functions, interaktive Dashboards, Logging, Chunking |

Jedes Notebook enthält Erklärungen, kommentierte Code-Beispiele und Übungsaufgaben.

Die Musterlösungen befinden sich in separaten **`*_Loesungen.ipynb`**-Dateien, die Teilnehmer bewusst öffnen müssen.

## Voraussetzungen

Die Notebooks werden über **Coder** bereitgestellt. Alle erforderlichen Pakete sind in der Umgebung vorinstalliert - keine lokale Installation notwendig.

Die Notebooks einfach in der Reihenfolge 01 bis 06 öffnen und ausführen.

## Pakete

| Paket | Verwendung |
|-------|------------|
| `pandas` | Datentabellen (DataFrames), ETL-Kern |
| `numpy` | Zahlenoperationen, fehlende Werte |
| `matplotlib` | Diagramme und Visualisierungen |
| `seaborn` | Statistische Diagramme (optional) |
| `openpyxl` | Excel-Dateien lesen und schreiben |
| `requests` | HTTP-Anfragen an REST-APIs |
| `plotly` | Interaktive Diagramme (optional) |
| `pyarrow` | Parquet-Dateiformat (Session2_Extras, optional) |

## Lernpfad

```
--- Session 1 ---                          --- Session 2 ---
Notebook 1 & 2          Notebook 3             Notebook 4             Notebook 5 & 6
Python-Grundlagen  -->  Daten einlesen  -->  Daten bereinigen  -->  Speichern & Visualisieren
      |                                                                       |
Session1_Extras                                                       Session2_Extras
  (optional)                                                            (optional)
```

## Weiterführende Ressourcen

| Ressource | Beschreibung | Link |
|-----------|-------------|------|
| **Python Dokumentation** | Offizielle Referenz zum Nachschlagen von Funktionen und Syntax | [docs.python.org](https://docs.python.org/3/) |
| **W3Schools Python** | Interaktive Tutorials mit "Try it yourself"-Beispielen | [w3schools.com/python](https://www.w3schools.com/python/default.asp) |
| **GeeksforGeeks Python** | Ausführliche Erklärungen und viele Beispiele | [geeksforgeeks.org/python](https://www.geeksforgeeks.org/python/python-programming-language-tutorial/) |

## Hinweise für Trainer

- Die `output/`- und `daten/`-Ordner werden zur Laufzeit automatisch von den Notebooks erstellt.
- Musterlösungen liegen als separate Dateien im Unterordner **`Loesungen/`** (z.B. `Loesungen/01_Python_Grundlagen_Loesungen.ipynb`). Teilnehmer müssen sie bewusst öffnen - in den Hauptnotebooks sind keine Lösungen enthalten.
- Alle Notebooks funktionieren offline. Lediglich das API-Beispiel in Notebook 3 benötigt eine Internetverbindung; es enthält einen Fallback für den Offline-Betrieb.
