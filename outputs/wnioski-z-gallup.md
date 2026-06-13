# Wnioski z Gallupa pod naukę AI i rozwój zawodowy

Twoje główne talenty:

1. Ukierunkowanie / Focus
2. Zgodność / Harmony
3. Analityk / Analytical
4. Bliskość / Relator
5. Uczenie się / Learner

Najważniejszy wniosek:

> Twój system nauki musi być prosty, projektowy i zabezpieczony przed rozproszeniem. Nie budujesz second brain. Budujesz system dowożenia umiejętności.

## Focus

### Jak wykorzystać

- Ustaw jedną główną oś: **Secure Enterprise AI Systems**.
- Pracuj na jednym głównym artefakcie tygodniowo.
- Każdy tydzień ma mieć jedno zdanie: "co ma istnieć na końcu tygodnia".
- Dashboard w Obsidianie ma pokazywać tylko: aktualny miesiąc, aktualny projekt, wynik tygodnia, 3 następne akcje i czego nie robić.

### Ryzyko

- Frustracja, gdy plan robi się zbyt szeroki.
- Przeskakiwanie między AUTOCOR, Pythonem, RAG, security, cloudem i frameworkami.

### Zabezpieczenie

- Tygodniowa lista `Do not do this week`.
- Maksymalnie jeden główny projekt naraz.
- Jeśli nowy temat nie wzmacnia AUTOCOR, Pythona, Secure RAG, AI Security albo portfolio, trafia do odłożonych.

## Harmony

### Jak wykorzystać

- Pasujesz do roli osoby łączącej klienta, security, infrastrukturę i biznes.
- Możesz być dobry w spokojnym tłumaczeniu ryzyk i szukaniu praktycznych kompromisów.
- W konsultingu i architekturze to duża przewaga, bo wiele problemów AI jest organizacyjno-technicznych.

### Ryzyko

- Możesz unikać trudnych ocen: "ten projekt ma zły model dostępu", "ten agent ma zbyt szerokie uprawnienia", "ten RAG może ujawniać dane".

### Zabezpieczenie

- Raz w tygodniu ćwicz krótką trudną wypowiedź techniczną:
  - "To rozwiązanie ma ryzyko data leakage, bo..."
  - "Nie wdrożyłbym tego bez ACL na retrievalu, bo..."
  - "Ten workflow wymaga human review, bo..."
- W review zapisuj jedno ryzyko, które trzeba nazwać wprost.

## Analytical

### Jak wykorzystać

- Idealnie pasuje do RAG evaluation, threat modelingu, debugowania, ADR-ów i architektury.
- Używaj pytań:
  - Dlaczego to działa?
  - Kiedy to się psuje?
  - Jaki jest trade-off?
  - Jak to przetestować?
  - Jakie są negatywne przypadki?

### Ryzyko

- Nadmierny research.
- Szukanie idealnego frameworka.
- Czytanie dokumentacji przez godzinę bez decyzji.

### Zabezpieczenie

- Limit researchu: **45 minut**.
- Po 45 minutach musi powstać jedno z:
  - decyzja,
  - eksperyment,
  - test,
  - ADR,
  - pytanie do późniejszego sprawdzenia.

## Relator

### Jak wykorzystać

- Lepszy będzie dla Ciebie mały krąg wartościowych kontaktów niż masowy networking.
- Szukaj 1:1 rozmów technicznych, feedbacku do projektów, mentorów i ludzi z podobnym kierunkiem.

### Ryzyko

- Możesz odkładać publiczną obecność i rozmowy rynkowe.
- Możesz czekać, aż portfolio będzie "idealne".

### Zabezpieczenie

- Co 2 tygodnie jedna mała interakcja:
  - pytanie techniczne do kogoś,
  - rozmowa 1:1,
  - prośba o review README,
  - krótki post z wnioskiem z projektu.

## Learner

### Jak wykorzystać

- Masz paliwo do długiego planu.
- Możesz regularnie uczyć się trudnych tematów: AUTOCOR, Python, RAG, AI security, cloud.

### Ryzyko

- Kolekcjonowanie kursów.
- Otwieranie nowych roadmap.
- Optymalizacja Obsidiana zamiast budowania projektów.

### Zabezpieczenie

- Kurs musi kończyć się artefaktem:
  - commit,
  - test,
  - diagram,
  - ADR,
  - README,
  - Anki cards,
  - case study note.
- Jeśli kurs nie daje artefaktu, nie wchodzi do planu.

## Twoja najlepsza metoda pracy

Najlepszy cykl:

> **Plan -> Recall -> Build -> Review**

Nie:

> "Czytam kurs i robię notatki."

Tak:

> "Ustalam artefakt, uczę się minimum, odtwarzam z pamięci, buduję, sprawdzam."

## Reguły antyrozproszeniowe

1. Nie zaczynam nowego kursu, jeśli obecny temat nie ma artefaktu.
2. Nie robię notatek bez active recall.
3. Nie dodaję do Anki kart, których nie rozumiem.
4. Nie uczę się drugiego frameworka agentowego, zanim LangGraph nie ma zastosowania w projekcie.
5. Nie poprawiam Obsidiana zamiast pisać kodu.
6. Nie robię researchu dłużej niż 45 minut bez decyzji albo eksperymentu.
7. Każdy tydzień kończy się dowodem: commit, test, diagram, ADR, README albo case study.

## Co mierzyć

Temat uznaj za opanowany dopiero, gdy spełniasz 4 z 5 warunków:

1. Potrafisz wyjaśnić temat z pamięci po 24-48 h.
2. Potrafisz użyć go w projekcie.
3. Potrafisz rozpoznać typowy błąd.
4. Potrafisz odróżnić go od podobnego pojęcia.
5. Potrafisz opisać ograniczenia, security risk albo trade-off.

Przykład:

Nie wystarczy:

> "Wiem, że Qdrant ma filtrowanie."

Wystarczy:

> "Potrafię zbudować kolekcję z metadanymi tenant/role, wykonać retrieval z filtrem, napisać test negatywny unauthorized retrieval i opisać, dlaczego filtrowanie musi zajść przed generacją odpowiedzi."

