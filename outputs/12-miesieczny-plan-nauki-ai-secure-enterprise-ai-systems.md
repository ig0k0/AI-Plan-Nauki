# 12-miesięczny plan nauki: Secure Enterprise AI Systems

Start: **16.06.2026**  
Okres: **16.06.2026 - 15.06.2027**  
Limit: **maksymalnie 14 h tygodniowo**  
Główny cel zawodowy: **Secure Enterprise AI Systems / AI Security & Implementation Architecture**  
Taktyczny cel początkowy: **AUTOCOR jako priorytet nr 1 na start**  
Drugi najważniejszy tor początkowy: **Python przez DataCamp, DeepLearning.AI i coddy.tech**

Zasada główna:

> Nie uczysz się kursów dla certyfikatów ukończenia. Uczysz się tylko tego, co wzmacnia AUTOCOR, Pythona, Secure RAG, AI Security albo portfolio.

## 1. Priorytety na rok

### Projekty główne

1. **Secure RAG Reference Architecture**  
   Główny projekt techniczny. Ma pokazać RAG, Qdrant, embeddings, metadata, evals, security, runbooki i architekturę enterprise.

2. **AI Security Test Harness for RAG**  
   Drugi główny projekt. Powinien być mocno powiązany z Secure RAG, najlepiej jako osobne repo albo osobny moduł/test suite, który testuje ten pierwszy projekt.

### Projekt pomocniczy / capstone

3. **AI Workflow Orchestrator**  
   Projekt pomocniczy, mniejszy zakres. Ma pokazać przepływ pracy, wywoływanie narzędzi, akceptację człowieka, dziennik audytu, retry i security by design. Nie musi być pełną produkcyjną integracją Slack/Linear.

### Dokument architektoniczny

4. **Local vs Cloud AI Architecture Review**  
   Dokument/studium przypadku, nie pełny projekt techniczny. Ma bazować na ADR-ach zbieranych od miesięcy 4-10.

### Laboratoria przygotowawcze

- `api-integration-lab` - laboratorium pomocnicze, nie główne repo do promowania.
- `llm-structured-output-lab` - laboratorium pomocnicze albo moduł w późniejszym projekcie, nie główne repo do promowania.

## 2. Stały rytm tygodnia

### Miesiące 1-4: AUTOCOR jest głównym celem

- 5-6 h: AUTOCOR.
- 3-4 h: Python przez DataCamp / coddy.tech / małe ćwiczenia.
- 2 h: DataCamp AI Fundamentals i podstawy AI.
- 1 h: GitHub, notatki, README, Obsidian.
- 1 h: angielski techniczny.

DeepLearning.AI wchodzi lekko dopiero wtedy, gdy zaczynasz LLM application basics.

### Miesiące 5-8: RAG i security stają się głównym celem

- 6 h: Secure RAG / AI Security Test Harness.
- 2-3 h: kursy pod aktualny etap.
- 1-2 h: Python i testy.
- 1 h: AUTOCOR utrzymaniowo, jeśli jeszcze niezdany.
- 1 h: dokumentacja, ADR-y, studium przypadku.
- 1 h: angielski techniczny.

### Miesiące 9-12: portfolio, architektura i rynek

- 5 h: dopracowanie projektów.
- 3 h: AI Workflow Orchestrator albo Local vs Cloud Architecture Review.
- 2 h: dokumentacja, studia przypadku, GitHub.
- 2 h: cloud/context architecture.
- 1 h: angielski.
- 1 h: rynek, CV, LinkedIn, rozmowy informacyjne.

## 3. Wątek poziomy: security od miesiąca 1

Security nie zaczyna się w miesiącu 7. Od pierwszego miesiąca każdy projekt i laboratorium ma mieć:

- `.env.example`,
- brak sekretów w repo,
- walidację danych wejściowych,
- walidację odpowiedzi modelu,
- minimalne uprawnienia,
- logging bez danych wrażliwych,
- `README` z sekcją `Security notes`,
- proste abuse cases,
- informację, kiedy wymagana jest weryfikacja człowieka,
- ograniczenia wywoływania narzędzi,
- threat notes nawet w małych labach.

Miesiące 7-8 są dopiero pogłębieniem: automatyzacja testów, OWASP, NIST, prompt injection, data leakage i raportowanie ryzyk.

## 4. Wątek poziomy: cloud od miesiąca 4

Cloud nie jest główną tożsamością, ale od pierwszego projektu RAG dokumentujesz decyzje architektoniczne:

- co zostaje lokalnie,
- co mogłoby iść do managed service,
- gdzie są dane wrażliwe,
- jakie są koszty,
- jakie są limity,
- jakie jest ryzyko vendor lock-in,
- co zmienia Bedrock / Vertex / Azure AI Foundry,
- jak wyglądałaby wersja hybrydowa.

ADR-y do tworzenia od miesięcy 4-10:

- `docs/adr/0003-local-vs-managed-vector-db.md`,
- `docs/adr/0004-openai-compatible-api-vs-managed-cloud-ai.md`,
- `docs/adr/0005-data-residency-and-sensitive-documents.md`,
- `docs/adr/0006-monitoring-and-cost-controls.md`.

Dokument `Local vs Cloud AI Architecture Review` w miesiącu 10 ma być podsumowaniem tych ADR-ów, nie pisaniem od zera.

## 5. Google Colab od początku

Od miesiąca 1 używasz **Google Colab** jako domyślnego środowiska do krótkich eksperymentów AI/Python.

Zasada:

- Colab do notatników, szybkich eksperymentów, embeddings, małych testów RAG i nauki.
- Lokalne repo do kodu, testów, dokumentacji i finalnych projektów.
- Nie trzymasz sekretów w notebookach.
- Nie wrzucasz danych firmowych do Colaba.
- Po 2-3 miesiącach oceniasz, czy Colab wystarcza.

Decyzja po miesiącu 3:

- Jeśli Colab wystarcza: kontynuujesz.
- Jeśli brakuje stabilności, prywatności albo wygody: przenosisz część eksperymentów lokalnie albo na mały VPS.
- Firmowy serwer GPU tylko do rzeczy zgodnych z celami firmy.

## Miesiąc 1: AUTOCOR + DataCamp AI Fundamentals + start Pythona

Cel: ustawić fundament i nie rozpraszać się. Na starcie najważniejszy jest AUTOCOR, drugi Python, a AI Fundamentals daje uporządkowane tło.

### Priorytety

1. AUTOCOR.
2. Python: DataCamp + coddy.tech.
3. DataCamp AI Fundamentals.
4. Google Colab jako środowisko eksperymentów.

### Czego się uczysz

AUTOCOR:

- automation concepts,
- APIs,
- programmability,
- Git/GitLab basics,
- model-driven programmability,
- telemetry na poziomie egzaminu.

Python:

- składnia,
- funkcje,
- pliki,
- JSON,
- błędy,
- proste requesty HTTP.

AI Fundamentals:

- czym jest AI,
- typy AI,
- mity vs fakty,
- gdzie AI daje wartość,
- przejście od problemu biznesowego do rozwiązania AI,
- podstawy LLM,
- odpowiedzialne użycie AI.

### Źródła

- DataCamp AI Fundamentals: `Foundations of Artificial Intelligence`.
- DataCamp: `Writing Functions in Python`.
- DataCamp: `Introduction to APIs in Python`.
- coddy.tech: codzienne krótkie ćwiczenia Python.
- Google Colab: pierwszy notebook `python-api-basics.ipynb`.

### Praktyka

Utwórz lokalnie `api-integration-lab`, ale traktuj je jako laboratorium.

Minimalny zakres:

- prosty klient API,
- `.env.example`,
- brak sekretów w repo,
- walidacja wejścia,
- logging bez danych wrażliwych,
- README po angielsku z `Security notes`.

### Kryterium ukończenia

- Masz rytm AUTOCOR.
- Masz pierwszy notebook Colab.
- Masz pierwsze małe repo/lab z README i notatkami security.

## Miesiąc 2: AUTOCOR + Python/API + AI Fundamentals cd.

Cel: wzmocnić praktyczne podstawy inżynierskie, ale bez robienia z `api-integration-lab` głównego projektu.

### Czego się uczysz

- Python: struktura kodu, moduły, błędy, logging.
- REST API: status codes, headers, auth basics.
- Testy: podstawy `pytest`.
- Docker: tylko minimum.
- AI Fundamentals: ChatGPT, przepływ pracy, prywatność, etyka, ML/LLM overview.

### Źródła

- DataCamp AI Fundamentals: `Interacting with ChatGPT`.
- DataCamp AI Fundamentals: `What is Machine Learning?`.
- DataCamp: `Software Engineering Principles in Python`.
- DataCamp: `Introduction to Testing in Python`.
- DataCamp: `Introduction to Git`.
- DataCamp: `Intermediate Git`.
- coddy.tech: Python daily practice.

Opcjonalnie:

- DataCamp: `Introduction to Docker`, tylko jeśli potrzebujesz do labu.

### Praktyka

Rozbuduj `api-integration-lab`:

- drugi klient API,
- testy błędów,
- retry/timeout,
- `.env.example`,
- `SECURITY.md` albo sekcja `Security notes`,
- threat notes: "co może pójść źle".

### Kryterium ukończenia

Masz lab pokazujący, że umiesz zrobić prostą integrację API w uporządkowany sposób, bez udawania, że to główne portfolio.

## Miesiąc 3: AUTOCOR + LLM application basics + decyzja o Colabie

Cel: wejść w LLM praktycznie, ale nadal trzymać AUTOCOR jako główny cel początkowy.

### Czego się uczysz

- LLM jako komponent systemu,
- tokeny,
- context window,
- hallucination,
- grounding,
- wyniki strukturalne,
- JSON/schema validation,
- fallback,
- error handling,
- proste prompt injection tests,
- logging decyzji modelu bez danych wrażliwych.

### Źródła

- DataCamp AI Fundamentals: `Introduction to Large Language Models`.
- DataCamp AI Fundamentals: `Introduction to Generative AI`.
- DataCamp AI Fundamentals: `AI Ethics`.
- DataCamp: `Large Language Models (LLMs) Concepts`.
- DataCamp: `Working with the OpenAI API`.
- DeepLearning.AI: `ChatGPT Prompt Engineering for Developers`.
- DeepLearning.AI: `Building Systems with the ChatGPT API`.
- coddy.tech: Python.

### Praktyka

`llm-structured-output-lab` traktuj jako lab albo moduł przyszłego RAG.

Zakres:

- prompt -> JSON,
- walidacja schematu,
- testy błędnych przypadków,
- proste testy prompt injection,
- fallback,
- flaga weryfikacji człowieka,
- README z ograniczeniami.

### Decyzja o Google Colab

Oceń:

- czy Colab wystarcza do nauki,
- czy nie przeszkadza w prywatności,
- czy przepływ pracy notebook -> repo jest wygodny,
- czy potrzebny jest lokalny runtime/VPS.

### Kryterium ukończenia

Masz podstawową aplikację/lab LLM i decyzję: Colab zostaje jako główne środowisko eksperymentów albo przechodzi do roli pomocniczej.

## Miesiąc 4: Secure RAG v0.1 + pierwsze ADR-y cloud/local

Cel: rozpocząć pierwszy główny projekt: **Secure RAG Reference Architecture**.

### Czego się uczysz

- embeddings,
- semantic search,
- vector DB,
- ingestion,
- chunking,
- metadata,
- retrieval,
- citations,
- podstawowy eval set.

### Źródła

- DataCamp: `Introduction to Embeddings with the OpenAI API`.
- DataCamp: `Retrieval Augmented Generation (RAG) with LangChain`.
- DeepLearning.AI: `Vector Databases: from Embeddings to Applications`.
- DeepLearning.AI: `Building Applications with Vector Databases`.
- Qdrant docs.

### Praktyka

Repo główne: `secure-rag-reference-architecture`.

Zakres v0.1:

- synthetic documents,
- ingestion,
- chunking,
- metadata,
- przykładowe klasy dokumentów,
- przykładowe role użytkowników,
- Qdrant,
- retrieval,
- odpowiedź ze źródłami,
- test braku źródeł,
- test unauthorized retrieval na prostym poziomie,
- szkic `docs/access-control-model.md`,
- `docs/adr/0003-local-vs-managed-vector-db.md`.

### Security od razu

Dodaj:

- `docs/security.md`,
- `docs/abuse-cases.md`,
- brak danych wrażliwych w logach,
- opis uprawnień danych,
- negatywny przykład: użytkownik próbuje pobrać dokument spoza swojej roli/tenanta.

### Kryterium ukończenia

Masz działający Secure RAG v0.1, a nie tylko tutorialowy RAG.

## Miesiąc 5: Secure RAG v0.2 + evaluation + risk register

Cel: podnieść Secure RAG do poziomu systemu ocenianego i dokumentowanego.

### Czego się uczysz

- Qdrant metadata filtering,
- reranking na poziomie koncepcyjno-praktycznym,
- eval set,
- Ragas albo własne proste evals,
- citation correctness,
- confidence,
- risk register,
- cloud/local trade-offs.

### Źródła

- DataCamp: `Developing LLM Applications with LangChain`.
- DataCamp: `Vector Databases for Embeddings with Pinecone`, tylko dla koncepcji vector DB.
- DeepLearning.AI: `Building and Evaluating Advanced RAG Applications`.
- DeepLearning.AI: `Retrieval Optimization: From Tokenization to Vector Quantization`.
- Ragas docs.
- Qdrant docs.

### Praktyka

Rozbuduj `secure-rag-reference-architecture`:

- eval set,
- podstawowe metryki jakości,
- test malicious document,
- test odpowiedzi bez źródeł,
- test unauthorized retrieval,
- `docs/access-control-model.md`,
- `docs/risk-register.md`,
- `docs/runbook.md`,
- `docs/adr/0004-openai-compatible-api-vs-managed-cloud-ai.md`.

`docs/access-control-model.md` powinien zawierać:

- role użytkowników,
- przykładowe klasy dokumentów,
- metadane dostępu,
- założenia tenant/user/document ACL,
- sposób filtrowania retrievalu,
- testy negatywne,
- opis ograniczeń.

### Kryterium ukończenia

Projekt ma działający RAG, testy jakości, podstawowe testy security, risk register i runbook.

## Miesiąc 6: Secure RAG v1 + studium przypadku

Cel: domknąć pierwszy główny projekt do wersji pokazowej.

### Czego się uczysz

- dokumentacja architektury,
- ADR,
- eval reporting,
- monitoring i cost notes,
- data residency,
- podstawy privacy-by-design.

### Źródła

- OWASP Top 10 for LLM Applications, orientacyjnie.
- NIST AI RMF, orientacyjnie.
- DeepLearning.AI: `Building and Evaluating Advanced RAG Applications`, domknięcie.
- Materiały cloud docs tylko pod ADR-y, bez certyfikatu.

### Praktyka

Domknij `secure-rag-reference-architecture`:

- `docs/architecture.md`,
- diagram,
- `docs/evaluation.md`,
- `docs/security.md`,
- `docs/access-control-model.md`,
- `docs/monitoring.md`,
- `docs/runbook.md`,
- `docs/adr/0005-data-residency-and-sensitive-documents.md`,
- `docs/adr/0006-monitoring-and-cost-controls.md`,
- pierwsze studium przypadku po angielsku.

Minimalne metryki w `docs/monitoring.md`:

- latency odpowiedzi,
- liczba zapytań bez źródeł,
- citation correctness pass rate,
- retrieval hit rate na eval set,
- liczba odmów / fallbacków,
- liczba przypadków wymagających weryfikacji człowieka,
- koszt per zapytanie, jeśli używasz płatnego API.

Nie musisz robić dużego Grafana dashboardu w pierwszym roku. Wystarczy prosty eksport metryk/logów i dokumentacja, jak te metryki byłyby monitorowane produkcyjnie.

### Checkpoint rynkowy

- Zaktualizuj LinkedIn headline.
- Dodaj projekt do GitHub jako "work in progress" albo opisz go bez nadmiernego marketingu.

### Kryterium ukończenia

Masz pierwszy główny projekt portfolio w wersji v1.

### Bufor realistyczny

Jeśli AUTOCOR zabiera więcej niż 4 h tygodniowo albo przygotowanie do egzaminu przeciąga się, Secure RAG v1 może przesunąć się z miesiąca 6 na miesiąc 7. Warunek: **v0.1 i v0.2 muszą być dowiezione**, a `docs/access-control-model.md`, podstawowe testy unauthorized retrieval i `docs/monitoring.md` nie mogą wypaść z zakresu.

## Miesiąc 7: AI Security Test Harness for RAG v0.1

Cel: rozpocząć drugi główny projekt, powiązany z Secure RAG.

### Czego się uczysz

- prompt injection,
- indirect prompt injection,
- malicious documents,
- data leakage,
- retrieval boundary tests,
- citation correctness,
- system prompt leakage,
- risk -> control -> test matrix.

### Źródła

- DeepLearning.AI: `Red Teaming LLM Applications`.
- DeepLearning.AI: `Improving Accuracy of LLM Applications`.
- OWASP Top 10 for LLM Applications.
- OWASP GenAI Security.
- NIST AI RMF.

### Praktyka

Repo główne lub moduł: `ai-security-test-harness-for-rag`.

Zakres v0.1:

- test prompt injection,
- test indirect prompt injection przez dokument,
- test data leakage,
- test unauthorized retrieval,
- test ACL/metadata filtering,
- test citation correctness,
- Markdown report,
- matrix: risk -> control -> test.

### Kryterium ukończenia

Masz test harness, który realnie testuje projekt Secure RAG.

## Miesiąc 8: AI Security Test Harness v1 + raport

Cel: pogłębić AI security i zrobić z tego niezależny artefakt portfolio.

### Czego się uczysz

- automatyzacja testów,
- raport HTML/Markdown,
- mapping OWASP/NIST,
- kontrole weryfikacji człowieka,
- ograniczenia guardrails,
- auditability.

### Źródła

- OWASP GenAI Security.
- NIST AI RMF.
- DataCamp: `Artificial Intelligence Governance`.
- DataCamp: `Responsible AI Practices`.
- DataCamp: `Responsible AI Data Management`.

### Praktyka

Rozbuduj `ai-security-test-harness-for-rag`:

- automatyczny raport,
- `docs/threat-model.md`,
- `docs/security-controls.md`,
- `docs/owasp-mapping.md`,
- przykładowy raport testów,
- studium przypadku po angielsku.

### Checkpoint rynkowy

- Opublikuj drugie studium przypadku.
- Zaktualizuj GitHub pinned repos.

### Kryterium ukończenia

Masz drugi główny projekt portfolio: AI Security Test Harness powiązany z Secure RAG.

## Miesiąc 9: AI Workflow Orchestrator jako mały capstone

Cel: pokazać automatyzację procesu biznesowego, ale bez budowania zbyt dużego produktu.

### Zakres minimalny

- testowe API Slacka,
- testowe API Lineara,
- deduplikacja,
- wynik strukturalny,
- akceptacja człowieka,
- dziennik audytu,
- retry,
- testy integracyjne,
- `docs/security-by-design.md`.

### Źródła

- DeepLearning.AI: `Functions, Tools and Agents with LangChain`.
- DeepLearning.AI: `AI Agents in LangGraph`.
- DataCamp: `Designing Agentic Systems with LangChain`.
- LangGraph docs.

Nie dokładaj:

- CrewAI,
- AutoGen,
- Semantic Kernel jako drugiego głównego frameworka,
- produkcyjnej integracji z prawdziwym Slackiem/Linearem, jeśli mocki wystarczą.

### Praktyka

Repo pomocnicze: `ai-workflow-orchestrator`.

Security od razu:

- ograniczone uprawnienia narzędzi,
- weryfikacja człowieka przed utworzeniem zgłoszenia,
- dziennik audytu,
- brak danych wrażliwych w logach,
- abuse cases.

### Kryterium ukończenia

Projekt jest ukończony, gdy można uruchomić jeden scenariusz end-to-end z testowymi wiadomościami: system pobiera wiadomość z testowego API Slacka, deduplikuje ją, generuje zgłoszenie jako wynik strukturalny, zatrzymuje go na akceptacji człowieka, po akceptacji zapisuje go przez testowe API Lineara, zapisuje dziennik audytu i pokazuje testy integracyjne dla tego przepływu.

## Miesiąc 10: Local vs Cloud AI Architecture Review

Cel: stworzyć dokument architektoniczny na bazie ADR-ów z projektów.

### Porównanie

- local AI,
- AWS Bedrock,
- Azure AI Foundry / AI-103 path,
- Google Vertex/Gemini,
- wariant hybrydowy.

### Dokument ma zawierać

- diagramy,
- koszty,
- latency,
- data residency,
- vendor lock-in,
- monitoring,
- security controls,
- rekomendację dla małej/średniej firmy,
- rekomendację dla środowiska enterprise.

### Źródła

- DataCamp: `Introduction to Amazon Bedrock`.
- DeepLearning.AI: `Serverless LLM Apps with Amazon Bedrock`.
- oficjalne docs AWS Bedrock / Azure AI Foundry / Google Vertex AI.
- ADR-y z miesięcy 4-9.

### Cert decision checkpoint

Nie zaczynasz jeszcze certyfikatu cloud, tylko wybierasz możliwy kierunek:

- Azure: **AI-103**, nie AI-102. Sensowny, jeśli Twoja praca lub rynek idą w Microsoft Foundry, Azure OpenAI, Copilot, agenty i enterprise Microsoft.
- AWS: Machine Learning Engineer Associate tylko jeśli faktycznie zrobisz praktykę z AWS/Bedrock/IAM/deployment/cost monitoring. To cert pod budowanie, operacjonalizację, wdrażanie i utrzymywanie ML workloads na AWS.
- Google: PMLE tylko jeśli wejdziesz mocniej w Vertex/Gemini i produkcjonalizację ML/AI. To cert o projektowaniu, budowaniu i produkcjonalizowaniu rozwiązań ML/AI, nie najkrótsza ścieżka do RAG/security.

Decyzja ma wynikać z tego, który cloud realnie wystąpił w projektach lub pracy, nie z tego, który cert wygląda najlepiej.

### Kryterium ukończenia

Masz dokument/studium przypadku, który wygląda jak próbka pracy AI Solutions Architect.

## Miesiąc 11: SQL / enterprise data jako dodatek do RAG

Cel: dodać enterprise data bez skręcania w pełny data engineering.

### Czego się uczysz

- SQL,
- Oracle SQL,
- ETL/ELT w Pythonie,
- CSV/SQL -> documents -> RAG,
- prosty SQL agent tylko z ograniczeniami,
- read-only user,
- allowlist tabel,
- logging zapytań.

### Źródła

- DataCamp: `Introduction to SQL`.
- DataCamp: `Intermediate SQL`.
- DataCamp: `Introduction to Oracle SQL`.
- DataCamp: `ETL and ELT in Python`.
- DeepLearning.AI: `Improving Accuracy of LLM Applications`, część z SQL agentem i ewaluacją.

### Praktyka

Dodaj do Secure RAG mały moduł:

- CSV/SQL -> dokumenty -> RAG,
- albo prosty SQL agent read-only,
- allowlist tabel,
- logging bez danych wrażliwych,
- `docs/security.md` z ryzykami.

### Kryterium ukończenia

Potrafisz pokazać, jak RAG/AI workflow łączy się z danymi enterprise bez niekontrolowanego dostępu do bazy.

## Miesiąc 12: Portfolio, rynek i decyzja o następnym certyfikacie

Cel: zamienić projekty w czytelny sygnał rynkowy.

### Co porządkujesz

- GitHub,
- README,
- studia przypadku,
- CV po angielsku,
- LinkedIn po angielsku,
- opis profilu zawodowego,
- ofertę konsultingową.

### Główne repozytoria do promowania

1. `secure-rag-reference-architecture`
2. `ai-security-test-harness-for-rag`
3. `ai-workflow-orchestrator` jako mniejszy capstone

### Dokument do promowania

- `local-vs-cloud-ai-architecture-review`

### Laboratoria jako pomocnicze

- `api-integration-lab`,
- `llm-structured-output-lab`.

Nie promuj ich jako głównych projektów. Mogą być linkowane jako "supporting labs".

### Checkpoint rynkowy

- 5-10 aplikacji testowych albo rozmów informacyjnych.
- Aktualizacja LinkedIn.
- CV pod role AI Security / AI Implementation / AI Automation.
- Oferta: `AI/RAG Security & Readiness Review`.

### Certyfikacja po roku

Rekomendacja:

- **AUTOCOR: tak, priorytet początkowy.**
- **Cloud cert: dopiero po 2 projektach portfolio.**
- **Azure: AI-103, nie AI-102.**
- **AWS: Machine Learning Engineer Associate tylko po praktyce z Bedrock/IAM/costs/deployment.**
- **Google: PMLE tylko jeśli chcesz wejść głębiej w Vertex/Gemini i MLOps.**

## Kontrola miesięczna

Na koniec każdego miesiąca odpowiedz w Obsidianie:

1. Jaki artefakt powstał?
2. Czy security było obecne od początku?
3. Czy dodałem `.env.example` i nie wrzuciłem sekretów?
4. Jakie abuse cases dopisałem?
5. Jakie ADR-y powstały?
6. Co z kursów faktycznie wykorzystałem?
7. Co było rozpraszaczem?
8. Co trafia do Anki?
9. Czy Colab nadal wystarcza?
10. Co zamykam w kolejnym miesiącu?

## Minimalny wynik, jeśli rok będzie trudny

Jeśli praca/studia ograniczą czas, minimalny sukces to:

1. AUTOCOR zdany albo bardzo blisko zdania.
2. `secure-rag-reference-architecture` v1.
3. `ai-security-test-harness-for-rag` v1.
4. `local-vs-cloud-ai-architecture-review`.
5. Jeden mniejszy `ai-workflow-orchestrator` albo dobrze opisany prototyp.
6. 2 studia przypadku po angielsku.

To nadal jest mocniejszy sygnał niż dużo kursów bez artefaktów.

## Czego nie robić przez ten rok

- Nie robić wielu frameworków agentowych równolegle.
- Nie robić pełnej ścieżki data science.
- Nie robić Kaggle jako głównego toru.
- Nie robić PyTorch/TensorFlow certów jako głównej inwestycji.
- Nie robić IBM AI Engineering jako głównej ścieżki.
- Nie robić prompt engineeringu jako osobnej tożsamości.
- Nie robić Cisco ponad AUTOCOR bez mocnego powodu finansowego.
- Nie robić głębokiego vLLM/KV cache/speculative decoding przed działającymi projektami RAG/security.
- Nie robić cloud certu przed dwoma projektami portfolio.
