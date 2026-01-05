# Analiza algoritmilor pentru descoperirea regulilor de asociere
## FP-Growth vs Apriori pe date FAO GIFT

Acest repository conține codul sursă utilizat pentru preprocesarea datelor
și extragerea regulilor de asociere din date reale privind consumul alimentar,
folosind algoritmul FP-Growth (alternativ) și Apriori (baseline).

## Autor
- Student: Tawadrous Mina  
- Coordonator: prof. Marian Crăciun

## Setul de date
- Sursă: FAO GIFT – Global Individual Food Consumption Data Tool
- Studiu de caz: Romania – 2012 – DIETA PILOT Adults Study
- Fișierul CSV nu este inclus în repository (dimensiune mare).
  Datele trebuie descărcate separat de pe platforma FAO și încărcate manual
  în Google Colab la rularea notebook-ului.

## Metodologie
- Curățarea și filtrarea datelor (eliminare valori lipsă și duplicări)
- Transformarea datelor în format tranzacțional (un coș alimentar per subiect)
- Extragerea regulilor de asociere folosind:
  - FP-Growth (algoritm alternativ)
  - Apriori (pentru comparație)
- Evaluarea regulilor prin metrici standard:
  support, confidence și lift

## Conținut repository
- `association_rules_fao.ipynb` – Notebook Google Colab cu întregul flux:
  preprocesare date, FP-Growth, Apriori, comparație și vizualizări
- `requirements.txt` – biblioteci necesare pentru rulare
- `README.md` – descrierea proiectului

## Rulare
1. Deschide fișierul `association_rules_fao.ipynb` în Google Colab
2. Încarcă fișierul CSV de consum alimentar (ex.: `consumption_user.csv`)
3. Rulează celulele în ordine

## Observații
Acest proiect este realizat în scop academic și respectă cerințele
privind livrabilele: raport PDF și cod sursă într-un repository.
