# System nauki: Obsidian, Anki, NotebookLM, Gallup

Cel:

> Obsidian ma być panelem sterowania nauką i projektami. Anki ma utrwalać pamięć. NotebookLM ma pomagać pracować ze źródłami. Nie budujesz second brain. Budujesz system dowożenia umiejętności.

## 1. Rola narzędzi

- **Obsidian**: plan tygodnia, decyzje, log projektu, przegląd. To jest centrum sterowania.
- **Anki**: pamięć długoterminowa.
- **NotebookLM**: praca z materiałami źródłowymi, streszczenia, pytania, porównania, szybkie wyjaśnienia. To nie jest centrum planowania.
- **GitHub/repo**: dowód kompetencji.
- **Google Colab**: szybkie eksperymenty Python/AI bez sekretów i bez danych firmowych.
- **Tablica/iPad**: architektura, debugging, threat modeling, recall wizualny.

Reguła:

> Obsidian trzyma decyzje i system. NotebookLM pomaga zrozumieć źródła. Anki utrwala to, co musi wracać z pamięci.

## 2. Główny przepływ pracy

Używaj cyklu:

> **Plan -> Recall -> Build -> Przegląd**

### Plan

Na początku tygodnia wybierasz jeden rezultat.

Przykład:

> Dodać timeout, retry i testy błędów do `api-integration-lab`.

Nie wpisujesz:

> Przerobić kilka kursów.

### Recall

Przed nauką:

- Co już wiem?
- Jak bym to wyjaśnił?
- Czego nie umiem?
- Jakie pytanie chcę rozwiązać?

Po nauce:

- zamknij materiał,
- zapisz 5 punktów z pamięci,
- zrób 3-5 fiszek,
- zapisz jedną akcję projektową.

### Build

Każda nauka ma kończyć się artefaktem:

- commit,
- test,
- diagram,
- ADR,
- README,
- notatka security,
- runbook,
- studium przypadku note.

### Przegląd

Raz w tygodniu sprawdzasz:

- co umiem odtworzyć bez notatek,
- co działa w repo,
- co było rozpraszaczem,
- co usuwam z planu,
- co idzie do Anki.

## 3. Dlaczego ten system ma sens naukowo

To rozwiązanie jest naukowo sensowne, bo opiera się na aktywnym przypominaniu, testowaniu, rozłożeniu nauki w czasie i metapoznaniu.

- **Practice testing / retrieval practice**: odtwarzanie wiedzy z pamięci wzmacnia późniejsze przypominanie bardziej niż samo ponowne czytanie.
- **Distributed practice / spaced repetition**: krótsze sesje rozłożone w czasie są zwykle skuteczniejsze niż jednorazowe intensywne uczenie.
- **Wyjaśnianie własnymi słowami**: pytania "dlaczego to działa?", "kiedy to się psuje?", "jak użyję tego w projekcie?" pomagają przejść od rozpoznawania do zrozumienia.
- **Metacognition**: planowanie, monitorowanie i ocena nauki pomagają unikać złudzenia, że "rozumiem, bo przeczytałem".
- **Project-based learning**: przy Twoim celu samo czytanie kursów ma niski zwrot. Dowodem umiejętności jest projekt, test, dokumentacja albo decyzja architektoniczna.

Wniosek praktyczny:

> Ten vault jest dobrym rozwiązaniem, jeśli pozostaje prosty. Gdy zaczniesz rozbudowywać tagi, pluginy, dashboardy i automatyzacje, system zacznie przeszkadzać.

## 4. Obsidian czy NotebookLM?

NotebookLM może być lepszy od Obsidiana do jednego zadania: pracy na źródłach. Według dokumentacji Google NotebookLM pozwala oprzeć odpowiedzi na wybranych źródłach, generować podsumowania, pytania i odpowiedzi z cytowaniami. To jest dobre przy kursach, PDF-ach, dokumentacji i długich materiałach.

NotebookLM nie jest lepszy jako główny system nauki, bo:

- nie powinien decydować, co jest priorytetem tygodnia,
- nie zastępuje logu projektu i decyzji architektonicznych,
- nie zastępuje GitHuba jako dowodu kompetencji,
- nie zastępuje Anki jako systemu powtórek,
- może dawać poczucie zrozumienia bez realnego recall.

Najlepszy układ dla Ciebie:

- **Obsidian**: dashboard, plan, decyzje, review, log projektu.
- **NotebookLM**: rozmowa z materiałami, generowanie pytań, sprawdzanie rozumienia, szybkie porównania.
- **Anki**: fiszki z rzeczy, które chcesz pamiętać bez pomocy narzędzi.

Zasada użycia NotebookLM:

1. Wrzuć tylko materiały do aktualnego tygodnia.
2. Poproś o 10 pytań sprawdzających.
3. Odpowiedz samodzielnie bez patrzenia.
4. Dopiero potem użyj NotebookLM do sprawdzenia luk.
5. Do Obsidiana przepisz tylko decyzję, wniosek albo akcję projektową.
6. Do Anki dodaj tylko 3-5 najlepszych pytań.

Nie wrzucaj do NotebookLM danych firmowych, sekretów, prywatnych tokenów, niepublicznego kodu ani materiałów, których nie możesz udostępnić usłudze zewnętrznej.

Źródła:

- Dunlosky et al., `Improving Students' Learning With Effective Learning Techniques`: https://journals.sagepub.com/doi/10.1177/1529100612453266
- Roediger & Karpicke, `Test-Enhanced Learning`: https://journals.sagepub.com/doi/10.1111/j.1467-9280.2006.01693.x
- EEF, `Metacognition and Self-Regulated Learning`: https://educationendowmentfoundation.org.uk/education-evidence/guidance-reports/metacognition
- The Learning Scientists, `Retrieval Practice`: https://www.learningscientists.org/blog/2016/6/23-1
- Google, `Introducing NotebookLM`: https://blog.google/innovation-and-ai/technology/ai/notebooklm-google-ai/
- Google, `NotebookLM Help`: https://support.google.com/notebooklm/

## 5. Dopasowanie do Gallupa

### Focus

Wykorzystanie:

- jeden główny cel,
- jeden główny rezultat tygodnia,
- jedna oś: Secure Enterprise AI Systems.

Ryzyko:

- frustracja przy zbyt wielu równoległych tematach.

Zabezpieczenie:

- tygodniowe `Nie robię`,
- maksymalnie jeden główny projekt naraz.

### Harmony

Wykorzystanie:

- dobra rola między biznesem, security, klientem i infrastrukturą.

Ryzyko:

- unikanie trudnych ocen technicznych.

Zabezpieczenie:

- raz w tygodniu zapisz jedno ryzyko wprost, np. "ten przepływ pracy wymaga weryfikacji człowieka, bo...".

### Analytical

Wykorzystanie:

- RAG evals,
- threat modeling,
- debugging,
- ADR-y.

Ryzyko:

- nadmierny research.

Zabezpieczenie:

- limit researchu: 45 minut, potem decyzja, eksperyment albo ADR.

### Relator

Wykorzystanie:

- mały krąg jakościowych kontaktów,
- rozmowy 1:1,
- prośby o feedback.

Ryzyko:

- odkładanie kontaktu z rynkiem.

Zabezpieczenie:

- jedna rozmowa techniczna lub prośba o feedback co 2 tygodnie.

### Learner

Wykorzystanie:

- energia do długiego planu.

Ryzyko:

- kolekcjonowanie kursów.

Zabezpieczenie:

- kurs musi skończyć się artefaktem. Inaczej nie wchodzi do planu.

## 6. Jak używać Obsidiana

Codziennie:

1. Otwórz `00_Dashboard.md`.
2. Sprawdź aktualny tydzień.
3. Zrób 5 minut recall.
4. Pracuj 60-90 minut.
5. Zapisz wynik, następną akcję i kandydatów do Anki.

Co tydzień:

1. Uzupełnij plik w `01_Plan`.
2. Wybierz jeden rezultat.
3. Zapisz zadania budowania.
4. Zapisz testy z pamięci.
5. Zrób przegląd w niedzielę.

Co miesiąc:

1. Uzupełnij plik w `04_Reviews`.
2. Linkuj dowód: commit, README, diagram, ADR, studium przypadku.
3. Zapisz rozpraszacze.
4. Wybierz jeden rezultat na kolejny miesiąc.

## 7. Jak używać Anki

Dodawaj:

- definicje,
- komendy,
- różnice między pojęciami,
- błędy, które popełniłeś,
- pytania z AUTOCOR,
- wzorce security,
- architekturę RAG,
- checklisty, które chcesz mieć w głowie.

Nie dodawaj:

- całych akapitów,
- długich list,
- wszystkiego "na później",
- kart, których nie rozumiesz.

Limit:

- 5-10 nowych kart dziennie,
- maksymalnie 40 nowych tygodniowo,
- 15-20 minut powtórek dziennie.

Tagi:

- `autocor`
- `python-api`
- `llm`
- `rag`
- `ai-security`
- `cloud`
- `english`

## 8. Reguły antyrozproszeniowe

1. Nie zaczynam nowego kursu, jeśli obecny temat nie ma artefaktu.
2. Nie robię notatek bez active recall.
3. Nie dodaję do Anki kart, których nie rozumiem.
4. Nie uczę się drugiego frameworka agentowego, zanim LangGraph nie ma zastosowania w projekcie.
5. Nie poprawiam Obsidiana zamiast pisać kodu.
6. Nie robię researchu dłużej niż 45 minut bez decyzji albo eksperymentu.
7. Każdy tydzień kończy się dowodem: commit, test, diagram, ADR, README albo studium przypadku.
8. Nie używam NotebookLM jako wymówki do biernego słuchania podsumowań bez recall.

## 9. Kiedy temat jest opanowany

Temat uznaj za opanowany, gdy spełniasz 4 z 5 warunków:

1. Potrafisz wyjaśnić go z pamięci po 24-48 h.
2. Potrafisz użyć go w projekcie.
3. Potrafisz rozpoznać typowy błąd.
4. Potrafisz odróżnić go od podobnego pojęcia.
5. Potrafisz opisać ograniczenie, ryzyko security albo trade-off.
