# Metody nauki i instrukcja korzystania z Obsidiana

Cel systemu:

> Obsidian ma być panelem sterowania nauką i projektami. Nie budujesz second brain. Budujesz system dowożenia umiejętności.

## 1. Uzasadnienie naukowe

Najlepiej dopasowane metody do Twojego planu:

- retrieval practice / active recall,
- spaced repetition,
- practice testing,
- self-explanation,
- interleaving,
- metacognition,
- project-based learning.

### Co potwierdza research

Dunlosky et al. ocenili `practice testing` i `distributed practice` jako techniki o wysokiej użyteczności. `Self-explanation` i `interleaved practice` ocenili jako umiarkowanie użyteczne, ale nadal sensowne w dobrych kontekstach. `Highlighting` i bierne `rereading` ocenili jako nisko użyteczne w porównaniu z aktywnym sprawdzaniem wiedzy.

Roediger i Karpicke pokazali efekt testowania: samo odtwarzanie materiału z pamięci poprawia późniejsze zapamiętanie bardziej niż samo ponowne studiowanie materiału. To pasuje do Twoich tematów, bo musisz nie tylko rozpoznawać pojęcia, ale umieć je zastosować w projekcie.

Spacing ma silne wsparcie w literaturze. W praktyce oznacza to Anki i powrót do tematów po kilku dniach oraz tygodniach, zamiast jednego długiego bloku "zakuwania".

EEF opisuje metacognition i self-regulated learning jako podejście oparte na planowaniu, monitorowaniu i ocenie uczenia się. Ważne: te strategie działają najlepiej, gdy są osadzone w konkretnym przedmiocie i zadaniu. Dlatego Twój Obsidian nie ma być osobnym systemem produktywnościowym, tylko prostym workflow wokół AUTOCOR, Pythona, RAG, AI Security i portfolio.

### Źródła

- Dunlosky et al., 2013, `Improving Students' Learning With Effective Learning Techniques`: https://journals.sagepub.com/doi/10.1177/1529100612453266
- Roediger & Karpicke, 2006, `Test-Enhanced Learning`: https://journals.sagepub.com/doi/10.1111/j.1467-9280.2006.01693.x
- EEF, `Metacognition and Self-Regulated Learning`: https://educationendowmentfoundation.org.uk/education-evidence/guidance-reports/metacognition
- The Learning Scientists, `Retrieval Practice`: https://www.learningscientists.org/blog/2016/6/23-1

## 2. Narzędzia i rola każdego z nich

- **Obsidian**: panel sterowania nauką i projektami.
- **Anki**: pamięć długoterminowa.
- **GitHub/repo**: dowód kompetencji.
- **Tablica/iPad**: myślenie wizualne, architektura, debugging, threat modeling.
- **Google Colab**: szybkie eksperymenty Python/AI, bez danych firmowych i bez sekretów.

## 3. Główny workflow: P-R-B-R

### Plan

Na początku tygodnia wybierasz jeden rezultat.

Nie:

> Przerobić 4 kursy.

Tak:

> Dodać retry/timeout i testy błędów do `api-integration-lab`.

### Recall

Przed nauką:

- Co już wiem?
- Jak bym to wyjaśnił?
- Czego nie umiem?
- Jakie pytanie chcę rozwiązać?

Po nauce:

- zamknij kurs/notatki,
- zapisz 5-10 punktów z pamięci,
- narysuj flow,
- zrób 3-5 fiszek,
- zapisz jedną akcję projektową.

### Build

Każdy blok nauki musi przejść do artefaktu:

- commit,
- test,
- README,
- diagram,
- ADR,
- Anki cards,
- case study note,
- security checklist,
- runbook.

### Review

Raz w tygodniu sprawdzasz:

- co umiem odtworzyć bez notatek,
- co działa w repo,
- czego Anki nie utrwaliło,
- co było rozpraszaczem,
- co usuwam z planu.

## 4. Minimalna struktura Obsidiana

Utworzony vault:

```text
AI-Learning-Vault/
  00_Dashboard.md
  INSTRUKCJA.md
  01_Plan/
    Week-2026-W24.md
  02_Projects/
    api-integration-lab.md
    secure-rag-reference-architecture.md
    ai-security-test-harness.md
    ai-workflow-orchestrator.md
    local-vs-cloud-ai-architecture-review.md
  03_Concepts/
    python-api.md
    oauth2-oidc.md
    rag-evaluation.md
    prompt-injection.md
    qdrant-metadata-filtering.md
  04_Reviews/
    Review-2026-06.md
  05_Templates/
    weekly-plan-template.md
    session-template.md
    concept-template.md
    project-log-template.md
    monthly-review-template.md
```

Nie dodawaj na start:

- PARA,
- Zettelkasten,
- Dataview,
- Kanban,
- rozbudowanych tagów,
- automatycznej synchronizacji z Anki,
- systemu "wszystko zapisuję".

## 5. Jak używać Obsidiana codziennie

Przed sesją:

1. Otwórz `00_Dashboard.md`.
2. Sprawdź `This week outcome`.
3. Zrób 5 minut recall.
4. Wybierz jedną sesję 60-90 minut.
5. Po sesji dopisz tylko wynik, next action i ewentualne Anki candidates.

Nie otwieraj najpierw:

- YouTube,
- nowych kursów,
- roadmap,
- pluginów Obsidiana,
- losowych artykułów.

Najpierw dashboard.

## 6. Jak robić notatki z kursów

Dla każdego modułu:

1. Przed lekcją zapisz 3 pytania.
2. Po lekcji zamknij materiał.
3. Napisz z pamięci 5 punktów.
4. Zrób 3-5 kart Anki.
5. Zrób jedną małą akcję w repo albo dokumentacji.

Przykład:

```markdown
## Pre-questions
1. Jak obsłużyć status code inny niż 200?
2. Gdzie trzymać API key?
3. Jak testować klienta API bez prawdziwego endpointu?

## Recall after lesson
- Request ma method, URL, headers, body.
- Response ma status code, headers, body.
- Błędy sieciowe trzeba obsłużyć osobno od błędów aplikacyjnych.
- Sekrety nie mogą trafić do repo.
- Testy powinny obejmować success, failure i timeout.

## Project action
Dodać do api-integration-lab:
- timeout,
- retry,
- test 500,
- test 429,
- .env.example.
```

## 7. Jak używać Anki

Anki ma być pamięcią długoterminową, nie drugim Obsidianem.

Dodawaj:

- definicje,
- komendy,
- różnice między podobnymi pojęciami,
- błędy, które popełniłeś,
- warunki użycia,
- wzorce security,
- pytania z AUTOCOR,
- elementy architektury RAG,
- checklisty, które chcesz mieć w głowie.

Nie dodawaj:

- całych akapitów,
- długich list 15-elementowych,
- notatek z kursu bez kontekstu,
- wszystkiego "bo może się przyda",
- kart, których nie potrafisz sformułować prosto.

Limit:

- 5-10 nowych kart dziennie,
- maksymalnie 40 nowych kart tygodniowo,
- powtórka codziennie 15-20 minut,
- jeśli Anki zajmuje ponad 25-30 minut dziennie, zmniejsz nowe karty.

Tagi:

- `autocor`
- `python-api`
- `llm`
- `rag`
- `ai-security`
- `cloud`
- `english`

## 8. Jak używać tablicy

Tablica ma utrzymywać Focus.

Stały układ:

```text
GŁÓWNY CEL:
Secure Enterprise AI Systems

TEN MIESIĄC:
[Miesiąc z planu]

TEN TYDZIEŃ:
[1 rezultat]

DZISIAJ:
[1 blok]

NIE ROBIĘ:
[3 rzeczy]

PYTANIE KONTROLNE:
Jaki artefakt powstaje z tej nauki?
```

Do problemów używaj:

```text
Problem:
Hipotezy:
1.
2.
3.

Test:
Wynik:
Decyzja:
```

## 9. Jak używać iPada

iPad to brudnopis techniczny, nie baza wiedzy.

Używaj do:

- rysowania architektury RAG,
- threat modelingu,
- mapowania zależności,
- przepisywania flow z pamięci,
- ćwiczenia wyjaśnienia po angielsku,
- analizy błędu krok po kroku.

Zasada:

> Z iPada do Obsidiana trafia tylko decyzja, diagram albo wniosek. Nie wszystko.

## 10. Minimalne pluginy Obsidiana

Na start:

- Templates,
- Daily Notes opcjonalnie, ale lepiej używać tygodniowych notatek,
- Calendar opcjonalnie,
- Git opcjonalnie,
- Excalidraw opcjonalnie, jeśli chcesz rysować w Obsidianie.

Nie instalować na start:

- Dataview,
- Tasks,
- Kanban,
- rozbudowanych systemów tagów,
- automatycznej synchronizacji z Anki,
- pluginów do Zettelkasten.

Powód: przy Learner + Analytical łatwo zamienić naukę AI w optymalizację Obsidiana.

## 11. Reguły antyrozproszeniowe

Wklej do Dashboardu:

```markdown
# Rules

1. Nie zaczynam nowego kursu, jeśli obecny temat nie ma artefaktu.
2. Nie robię notatek bez active recall.
3. Nie dodaję do Anki kart, których nie rozumiem.
4. Nie uczę się drugiego frameworka agentowego, zanim LangGraph nie ma zastosowania w projekcie.
5. Nie poprawiam Obsidiana zamiast pisać kodu.
6. Nie robię researchu dłużej niż 45 minut bez decyzji albo eksperymentu.
7. Każdy tydzień kończy się dowodem: commit, test, diagram, ADR, README albo case study.
```

