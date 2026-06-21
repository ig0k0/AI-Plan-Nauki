# Instrukcja korzystania z vaulta

Ten vault jest prostym panelem sterowania nauką. Nie jest second brain.

## Ocena struktury

Struktura jest dobra, jeśli używasz jej jako prostego systemu dowożenia:

- `00_Dashboard.md` mówi, na czym skupiać uwagę teraz.
- `01_Plan/` trzyma tydzień i wynik tygodnia.
- `02_Projects/` trzyma log projektów i decyzje.
- `03_Concepts/` trzyma tylko pojęcia, które wracają w projektach.
- `04_Reviews/` trzyma przeglądy tygodnia/miesiąca.
- `05_Templates/` przyspiesza tworzenie notatek.

Nie dodawaj nowych folderów, dopóki obecne nie przestaną wystarczać.

## Rola narzędzi

- Obsidian: plan, decyzje, log projektu, przegląd.
- NotebookLM: praca z materiałami źródłowymi i pytania sprawdzające.
- Anki: pamięć długoterminowa.
- GitHub: dowód kompetencji.

## Codzienny start

1. Otwórz `00_Dashboard.md`.
2. Sprawdź `Wynik tego tygodnia`.
3. Zrób 5 minut recall.
4. Pracuj 60-90 minut nad jednym blokiem.
5. Jeśli używasz NotebookLM, poproś o pytania sprawdzające, nie tylko streszczenie.
6. Na koniec dopisz:
   - co powstało,
   - następną akcję,
   - 3-5 kandydatów do Anki.

## Co tydzień

1. Utwórz albo zaktualizuj plik w `01_Plan/`.
2. Wybierz jeden główny rezultat.
3. Zapisz zadania budowania.
4. Zapisz testy z pamięci.
5. Zapisz źródła do NotebookLM tylko dla aktualnego tygodnia.
6. W niedzielę zrób przegląd.

## Co miesiąc

1. Utwórz plik przeglądu w `04_Reviews/`.
2. Zapisz realny artefakt.
3. Linkuj commit, README, diagram, ADR albo studium przypadku.
4. Usuń rozpraszacze z kolejnego miesiąca.

## Co trafia do Obsidiana

- decyzje,
- pytania,
- recall,
- self-explanation,
- ADR-y,
- log projektu,
- przegląd,
- linki do commitów,
- kandydaci do Anki.

## Co trafia do NotebookLM

- materiały kursowe z aktualnego tygodnia,
- dokumentacja techniczna,
- PDF-y i długie artykuły,
- własne krótkie notatki do sprawdzenia.

Do NotebookLM nie wrzucaj sekretów, tokenów, danych firmowych, prywatnego kodu ani materiałów, których nie możesz udostępnić usłudze zewnętrznej.

## Co nie trafia do Obsidiana

- pełne transkrypcje kursów,
- skopiowane akapity z dokumentacji,
- wszystko "bo może się przyda",
- rozbudowane tagi,
- losowe linki bez decyzji.

## Minimalny przepływ z NotebookLM

1. Dodaj tylko źródła z aktualnego tygodnia.
2. Poproś o 10 pytań sprawdzających.
3. Odpowiedz samodzielnie.
4. Sprawdź odpowiedzi w NotebookLM.
5. Do Obsidiana zapisz tylko decyzję, lukę albo akcję.
6. Do Anki dodaj tylko najlepsze pytania.
