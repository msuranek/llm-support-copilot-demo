# llm-support-copilot-demo

Prototyp support copilotu postaveného na LLM — retrieval, guardrails a eskalace na člověka.

## O projektu

Tady jsem si ověřoval základní přístup: LLM nepíše odpovědi zákazníkům přímo, ale připravuje návrh pro agenta. Agent schválí, upraví nebo eskaluje. Výsledkem je rychlejší práce agenta bez rizika plně autonomních odpovědí.

Projekt jsem postavil jako experiment, ze kterého jsem se hodně naučil — zejména co se týče fallbacků, logování a monitoring latence. Bez těhle věcí vypadá demo dobře, ale v produkci to vydrží krátce.

## Architektura

- `docs/architecture.md` — komponenty a datový tok
- `docs/evaluation.md` — hodnoticí kritéria, fallback scénáře, edge cases

## Tok zpracování

1. Přijde support ticket nebo chat zpráva.
2. Systém identifikuje záměr a načte relevantní kontext.
3. LLM připraví návrh odpovědi pro agenta.
4. Guardrails zkontrolují návrh na rizikové vzory nebo nejistotu.
5. Agent schválí, upraví nebo eskaluje.

## Co to není

- Produkčně nasaditelná aplikace.
- Doporučení nahradit lidi v high-stakes supportu.

## License

MIT — viz LICENSE
