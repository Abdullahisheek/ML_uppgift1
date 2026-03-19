# ML Uppgift 1 – California Housing

## Syfte
Syftet med denna uppgift är att bygga en maskininlärningsmodell som kan förutsäga bostadspriser (median_house_value) baserat på data från California Housing-datasetet.

## Metod
Arbetet följer ett enkelt ML-flöde:
- Data lästes in och analyserades (EDA)
- Saknade värden hanterades genom att ta bort rader
- Kategoriska variabler (ocean_proximity) togs bort
- Datan delades upp i tränings- och testdata
- Tre modeller testades:
  - DummyRegressor (baseline)
  - Linear Regression
  - Random Forest

Modellerna jämfördes med hjälp av RMSE och cross-validation.

## Resultat
Random Forest presterade bäst med lägst RMSE och valdes som slutlig modell.  
Modellen optimerades även med GridSearchCV för att förbättra prestandan.


## Slutsats
Random Forest är den mest lämpliga modellen i denna uppgift eftersom den kan hantera mer komplexa samband i datan jämfört med enklare modeller.

## Begränsningar
- Den kategoriska variabeln ocean_proximity användes inte
- Modellen bygger på historisk data
- Ytterligare optimering och feature engineering kan förbättra resultatet

## Filer i projektet
- `ML_Uppgift1_Abdullahi_Sheek.ipynb` – Notebook med hela analysen
- `ML Uppgift 1 – California Housing.pdf` – Kort rapport

## Hur man kör projektet
1. Installera dependencies:

pip install -r requirements.txt


2. Kör notebooken i Jupyter/VS Code