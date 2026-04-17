# llm-support-copilot-demo

Ukázkový návrh AI copilot workflow pro zákaznickou podporu.

## Cíl

Ukázat, jak může LLM pomáhat support týmu bez toho, aby bezhlavě odpovídal zákazníkům. Repozitář
je koncipovaný jako demo architektura a obsahový základ pro:

- technický článek
- demo prezentaci
- GitHub showcase repo

## Co repo demonstruje

- retrieval nad interní knowledge base
- návrh odpovědi pro agenta
- guardrails pro citlivé nebo nejisté situace
- eskalaci na člověka

## Obsah repozitáře

- `docs/architecture.md`:
  přehled komponent a toku dat
- `docs/evaluation.md`:
  jak hodnotit kvalitu draftů a kdy odpověď nepustit dál

## Typický workflow

1. Přijde ticket nebo chat.
2. Systém určí intent a získá relevantní kontext.
3. LLM připraví draft odpovědi.
4. Guardrails zkontrolují rizikové vzory.
5. Agent odpověď schválí, upraví nebo eskaluje.

## Proč je to silné pro osobní brand

Téma support copilotů je dost praktické, srozumitelné i pro netechnické publikum a zároveň ukazuje,
že AI nasazuješ s důrazem na workflow, ne jen na generování textu.
