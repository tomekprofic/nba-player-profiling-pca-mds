# NBA Player Profiling: PCA & MDS Analysis

## Opis projektu
Projekt poświęcony jest zaawansowanej analizie statystycznej zawodników ligi NBA grających na pozycji środkowego (Center) w sezonie 2022/2023. Głównym celem było zbadanie podobieństw między graczami oraz identyfikacja kluczowych czynników różnicujących styl gry na tej pozycji przy użyciu technik redukcji wymiarowości.

## Metodyka i narzędzia
W projekcie wykorzystano dwie komplementarne techniki statystyczne:
1. **Analiza Głównych Składowych (PCA):** Pozwoliła na redukcję 12 zmiennych opisujących osiągnięcia zawodników do 3 głównych wymiarów wyjaśniających ponad 78% całkowitej wariancji.
2. **Skalowanie Wielowymiarowe (MDS / Sammon Mapping):** Posłużyło do wizualizacji relacji podobieństwa między graczami w przestrzeni 2D i 3D.

**Stack technologiczny:**
- **Język:** R
- **Kluczowe biblioteki:** `psych`, `factoextra`, `MASS`, `ggplot2`, `rgl` (wizualizacje 3D).

## Kluczowe wyniki
### Interpretacja Składowych (PCA)
* **PC1 (53,8%): Oś Jakości/Wolumenu** – oddziela supergwiazdy (Embiid, Jokić) od zawodników zadaniowych.
* **PC2 (13,6%): Oś Stylu Gry** – polaryzacja na nowoczesnych środkowych ("Stretch Five" – rzuty za 3 pkt) oraz tradycyjnych ("Paint Beasts" – dominacja pod koszem).
* **PC3 (10,8%): Oś Wpływu (Impact)** – odzwierciedla realny wpływ gracza na zwycięstwa zespołu (wskaźnik +/-).

### Skalowanie (MDS)
* Uzyskano bardzo wysokie dopasowanie modelu w 3 wymiarach (**STRESS ≈ 1,1%**), co oznacza niemal idealne odwzorowanie realnych różnic statystycznych między zawodnikami.
* Zidentyfikowano unikalne klastry graczy, m.in. elitę ligi oraz grupy graczy o niemal identycznych profilach statystycznych.

## Zawartość repozytorium
* `Projekt2_SAD.Rmd` – kompletny kod źródłowy analizy w R Markdown.
* `Projekt2_SAD.pdf` – pełna wersja raportu z interpretacją wyników.
* `2023_nba_player_stats.csv` – zbiór danych wejściowych.

---
*Projekt zrealizowany w ramach przedmiotu Statystyczna Analiza Danych.*
