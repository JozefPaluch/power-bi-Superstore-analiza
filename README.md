# Analiza Sprzedaży w Stanach Zjednoczonych (Plik Superstore)

# Cel projektu
Analiza wyników sprzedaży i zyskowności fikcyjnego sklepu Superstore. Projekt pokazuje trendy czasowe, rozkład geograficzny zysków oraz kluczowe wskaźniki KPI.

# Technologie oraz umiejętności
- Power BI Desktop: Wizualizacja danych i budowa dashboardu.
- Power Query: Czyszczenie danych (zmiana typów, obsługa ustawień regionalnych dla walut).
- DAX: Tworzenie miar obliczeniowych (`Total Sales`, `Total Profit`, `Profit Margin`).
- Modelowanie danych: Stworzenie relacji między tabelą kalendarza a danymi sprzedaży.

# Kluczowe miary DAX
W projekcie wykorzystałem m.in.:
- `Total Sales = SUM(superstore[Sales])`
- `Total Profit = SUM(superstore[Profit])`
- `Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)`

# Wnioski z analizy
- Najwyższe skoki sprzedaży są odnotowywane w czwartym kwartale każdego roku, co jest efektem sezonu świątecznego. Sugeruje to konieczność wzmocnienia logityki i zapasów w tym okresie.
- Kategoria Technology generuje najwyższy zysk netto, mimo że nie jest najczęściej kupowaną kategorią. Z kolei kategoria Furniture, mimo wysokich obrotów, ma najniższą marżę.
- Region Zachodni jest najbardziej dochodowy, głównie dzięki świetnym wynikom w stanie Kalifornia. Z kolei niektóre stany w regionie centralnym wykazują stratę, co może chociażby wynikać ze zbyt agresywnej polityki rabatowej.
- Analiza pokazuje, że rabaty powyżej 20% rzadko przekładają się na wzrost zysku. Znacząco zwiększają wolumen sprzedaży, znosząc przy tym zbyt mocno marżę produktu.
