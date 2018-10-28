# Rozpoznanie problemu

Zagadnienie rozpoznawania maszynowego faktur jest utrudnione o tyle, że firmy stosują ich różne formaty. Jednak zastosowanie odpowiednich narzędzi pozwala z większą lub mniejszą dokładnością przewidzieć ich treść. Zwyczajowy rozkład informacji zawartych w fakturze zawsze pozostaje taki sam.

# Stosowane narzędzia

- Język R – język programowania, stworzony na potrzeby uczenia maszynowego.
- Tesseract – silnik optycznego rozpoznawania znaków utworzony i rozwijany przez Google.
- Naiwny klasyfikator bayesowski – klasyfikator probabilistyczny oparty na założeniu niezależności zmiennych. Naiwny, ponieważ zmienne nie zawsze mają związek z rzeczywistością.
- Accord.NET – framework open source do uczenia maszynowego.

# Potrzebne dane

Faktury zawierają specyficzne dane, które muszą zostać odpowiednio rozpoznane przez system. Są to:
- Liczba pozycji na fakturze.
- Jednostki stosowane przy do określenia wartości.
- Cena jednostkowa.
- Waluta.
- Informacje o produkcie.
- Termin płatności.

# Cel projektu

Głównym celem jest stworzenie prototypu oprogramowania do rozpoznania i przetworzenia informacji zawartych w fakturach. W tym celu konieczne jest wykonanie następujących czynności:

**Badanie powinno wykazać:**
- Istniejące silniki OCR pod względem ich skuteczności w rozpoznawaniu słów na fakturach.
- W jaki sposób można zastosować dopasowanie tekstu w celu wydobycia danych strukturalnych ze zwykłego tekstu i poprawienia błędów generowanych przez OCR.
- W jaki sposób proces interpretacji faktur zostanie zautomatyzowany za pomocą uczenia maszynowego na danych specyficznych dla faktury.

**Wdrożenie silnika OCR powinno:**
- Popełniać niewiele błędów.
- Wytwarzać czytelny zwykły tekst.
- Zachować strukturę faktur.

**Implementacja uczenia maszynowego powinna:**
- Wykazać, czy dane w fakturach są prawidłowe, czy powinny być nadzorowane i poprawiane ręcznie.
- Być modułowa, aby ułatwić dostosowanie rozwiązania do przyszłych dziedzin.
- Określić procentowo, stopień poprawności faktury.

**Analiza powinna:**
- Ocenić, w jaki sposób istniejące silniki OCR działają na różnych fakturach.
- Stwierdzić, czy prototyp maszyny do nauki staje się lepszy pod wpływem ilości przetwarzanych danych.
- Obliczyć, z jaką pewnością protokół uczenia maszynowego dostarczy odpowiedź.
- Ocenić, czy technika jest działającą alternatywą dla ludzkiego nadzoru.

# Utrudnienia projektowe
- Trudności w rozpoznawaniu tekstu odręcznego.
- Rozpoznawanym językiem będzie jedynie język polski i angielski.
