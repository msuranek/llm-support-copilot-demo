# Architecture Overview

## Komponenty

- Ticket ingest:
  přijímá vstup ze support kanálu
- Intent classifier:
  určuje typ dotazu a prioritu
- Retrieval layer:
  hledá odpovědi v interní dokumentaci nebo FAQ
- LLM response draft:
  připraví návrh odpovědi pro operátora
- Guardrails:
  zachytí nejisté, citlivé nebo rizikové výstupy
- Human review:
  člověk výstup schválí nebo upraví

## Princip

LLM není finální autorita. Je akcelerátor práce support agenta.

## Kde vzniká hodnota

- rychlejší první draft
- menší přepínání mezi systémy
- konzistentnější odpovědi
- lepší onboarding juniorních agentů
