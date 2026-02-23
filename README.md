# 📊 Data Science & Business Analytics Portfolio


To repozytorium stanowi centralny hub dokumentacji moich projektów analitycznych. Wykorzystuję tutaj podejście **Documentation-as-Code**, budując interaktywną stronę za pomocą MkDocs i automatyzując wdrożenie przez CI/CD.

## 🔗 Live Demo
Z pełną, czytelną wersją dokumentacji projektowej zapoznasz się tutaj:
 **[https://c8nraad.github.io/Portfolio-Data-Sience/](https://c8nraad.github.io/Portfolio-Data-Sience/)**

---

## 🛠️ Stack Techniczny Portfolio
* **Dokumentacja:** MkDocs z motywem `material`.
* **Analiza Danych:** Python (Pandas, NumPy).
* **Automatyzacja:** GitHub Actions (automatyczny build przy każdym `push`).
* **Integracje:** OCR Pipeline, GPT-4o API, SQLite.

## 📈 Kluczowe Projekty (Case Studies)

### 1. AI Invoice Intelligence (Multimodal ETL)
Zaawansowany rurociąg danych typu **Extract-Transform-Load**.
* **Problem:** Niestrukturalne dane z faktur PDF/JPG.
* **Rozwiązanie:** Wykorzystanie modelu GPT-4o (Vision) do ekstrakcji danych prosto do obiektów Pythona (Pydantic).
* **Data Engineering:** Łączenie danych przy użyciu **Vectorized Joins** w Pandas z bazą klientów SQLite.

### 2. Analiza Ryzyka Ubezpieczeniowego
Przetwarzanie i czyszczenie dużych zbiorów danych biznesowych.
* **Technologie:** Pandas, Matplotlib.
* **Wartość:** Identyfikacja kluczowych czynników wpływających na rentowność portfela.

---

## 🏗️ Struktura Projektu
- `docs/` - Pliki źródłowe Markdown z opisami projektów.
- `mkdocs.yml` - Główna konfiguracja wizualna.
- `.github/workflows/` - Skrypty automatyzacji wdrożenia.