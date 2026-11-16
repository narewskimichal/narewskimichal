[English](https://github.com/narewskimichal) · Polski

# Michał Narewski

**Informatyka i ekonometria (studia magisterskie)** · AGH w Krakowie · Analiza danych · Analiza finansowa · Księgowość

Analizuję dane w Pythonie, SQL, Power BI i R, najczęściej przy problemach związanych z finansami: ceny mieszkań, ryzyko portfela i strategie inwestycyjne. 

Każdy projekt poniżej ma własne README z pytaniami, wykresami i głównymi wynikami aby w kilka minut można się zorientować, o co w nim chodzi.

## Narzędzia

- **Python:** pandas, NumPy, scikit-learn, XGBoost, TensorFlow/Keras, matplotlib, Jupyter
- **SQL:** PostgreSQL, modelowanie danych, zapytania analityczne
- **Power BI:** ETL w Power Query, DAX, model danych, wizualizacja danych, dashboardy
- **Excel:** Power Query, tabele przestawne, XLOOKUP, SUMIFS, tablice dynamiczne, formatowanie warunkowe, VBA
- **R:** szeregi czasowe i modele ekonometryczne (GARCH, DCC-GARCH, BEKK), ggplot2
- **Inne:** Copilot Studio, Git i GitHub, VS Code

## Business intelligence i wizualizacja danych

### [Dostępność mieszkań w Polsce](https://github.com/narewskimichal/poland-housing-affordability)
**Python** (czyszczenie danych) · **PostgreSQL** (SQL) · **Power BI** (ETL, DAX, dashboard) · **Copilot Studio** (agent AI)

- **Repozytorium:** [poland-housing-affordability](https://github.com/narewskimichal/poland-housing-affordability)
- **Pytanie:** ile metrów kwadratowych mieszkania można kupić za średnią pensję w 15 polskich miastach i czy taniej jest kupić, czy wynająć?
- **Wynik:** za jedno przeciętne miesięczne wynagrodzenie brutto można kupić **1,19 m² w Katowicach**, ale tylko **0,60 m² w Warszawie**, a rata kredytu za typowe mieszkanie jest **wyższa od czynszu najmu we wszystkich 15 miastach**.
- **W środku:** [Python](https://github.com/narewskimichal/poland-housing-affordability/tree/main/python) · [SQL](https://github.com/narewskimichal/poland-housing-affordability/tree/main/sql) · [Power BI](https://github.com/narewskimichal/poland-housing-affordability/tree/main/powerbi) · [Copilot Studio](https://github.com/narewskimichal/poland-housing-affordability/tree/main/copilot)

### [Raport wiekowania należności w Excelu](https://github.com/narewskimichal/ar-aging-report)
**Excel** (ETL w Power Query, tabele przestawne, XLOOKUP, tablice dynamiczne) · **VBA** (automatyzacja) · **Python** (dane syntetyczne)

- **Repozytorium:** [ar-aging-report](https://github.com/narewskimichal/ar-aging-report)
- **Pytanie:** jak przez 12 miesięcy zmieniają się należności, udział przeterminowanych i DSO, i których klientów windykować w pierwszej kolejności?
- **Wynik:** należności wzrosły z **2,28 do 3,15 mln EUR**, udział przeterminowanych z **21% do 38%**, a DSO z **41,5 do 53,6 dnia**. Jeden kluczowy klient przekracza limit kredytowy o **83%**.
- **W środku:** [Raport w Excelu](https://github.com/narewskimichal/ar-aging-report/tree/main/excel) · [Kod VBA](https://github.com/narewskimichal/ar-aging-report/blob/main/excel/vba/ReportMacros.bas) · [Raport PDF](https://github.com/narewskimichal/ar-aging-report/blob/main/excel/output/AR_report_2026-10.pdf)

## Ekonometria finansowa

### [Portfel minimalnej wariancji na GPW](https://github.com/narewskimichal/mvp-portfolio-gpw)
**R** · optymalizacja portfela · modele DCC-GARCH i BEKK · backtesting · projekt uczelniany

- **Repozytorium:** [mvp-portfolio-gpw](https://github.com/narewskimichal/mvp-portfolio-gpw)
- **Pytanie:** czy zaawansowane modele kowariancji zmniejszają ryzyko portfela 5 spółek GPW (PZU, BNP Paribas, CD Projekt, Orange Polska, Orlen) w porównaniu z kowariancją próbkową? Backtest 2019–2025, 350 przebudów portfela.
- **Wynik:** **nie**. Zmienność portfela wyniosła **21,4%** przy kowariancji próbkowej i **21,2%** przy DCC-GARCH, a BEKK okazał się najbardziej ryzykowny: **22,7%**.

### [Backtest Value-at-Risk z modeli GARCH dla Apple](https://github.com/narewskimichal/garch-var-backtest-aapl)
**R** · szeregi czasowe · modele zmienności GARCH · backtest VaR (testy Kupca i Christoffersena) · projekt uczelniany

- **Repozytorium:** [garch-var-backtest-aapl](https://github.com/narewskimichal/garch-var-backtest-aapl)
- **Pytanie:** który z 9 modeli typu GARCH daje wiarygodne prognozy 95% VaR dla Apple przy oknach kroczących 100, 200 i 500 dni?
- **Wynik:** **długość okna miała większe znaczenie niż wybór modelu**. Przy 500 dniach test Kupca przeszło **8 z 9 modeli**, przy 100 dniach **żaden**. EGARCH najlepiej dopasował się do całej próby, ale w prognozach był najmniej wiarygodny.

## Uczenie maszynowe (praca magisterska)

### [Uczenie maszynowe a Buy & Hold na BTC](https://github.com/narewskimichal/btc-ml-vs-buy-and-hold)
**Python** · **uczenie maszynowe** (XGBoost, regresja logistyczna, LSTM) · walidacja walk-forward · backtesting 

- **Repozytorium:** [btc-ml-vs-buy-and-hold](https://github.com/narewskimichal/btc-ml-vs-buy-and-hold)
- **Pytanie:** czy reguły inwestycyjne oparte na uczeniu maszynowym wygrywają z kupieniem i trzymaniem BTC? Powtórzone na SPY, TLT i ETH.
- **Wynik:** na BTC adaptacyjna strategia XGBoost zmniejszyła maksymalne obsunięcie kapitału z **−77% do −30%** i podniosła wskaźnik Sharpe'a z **0,53 do 0,77**. Poprawa Sharpe'a **nie jest istotna statystycznie** (p = 0,43) i nie powtarza się na pozostałych aktywach.
- **W środku:** [Notatnik z wynikami](https://github.com/narewskimichal/btc-ml-vs-buy-and-hold/blob/main/analysis.ipynb) · [Kod pracy](https://github.com/narewskimichal/btc-ml-vs-buy-and-hold/tree/main/thesis_code)

## Kontakt

Jeśli któryś projekt Cię zainteresował, napisz do mnie na [LinkedIn](https://www.linkedin.com/in/michal-narewski).
