# 08 – Aplicació al TFG: Plataforma distribuïda per a ulleres mèdiques amb IA

Aquesta secció integra tots els conceptes de sistemes distribuïts estudiats
en aquesta wiki aplicant-los al projecte del TFG: una plataforma d’ulleres
mèdiques amb IA, orientada a baixa latència, alta disponibilitat i seguretat.

## Objectius d’aquesta secció

- Connectar la teoria amb la implementació real.
- Justificar cada decisió d’arquitectura del TFG.
- Documentar fluxos, models de dades i protocols utilitzats.
- Explicar com es garanteix la seguretat i la disponibilitat.
- Crear la base del capítol tècnic del TFG.

## Continguts previstos

- Arquitectura general del sistema
- Paper de l’orquestrador (M5)
- Sincronització entre ulleres i microserveis
- Gestió de logs clínics (Lamport, vectorial, etc.)
- Tolerància a fallades en entorns clínics
- Replicació i consistència eventual controlada
- Elecció de lideratge (Raft)
- Autenticació híbrida (Kerberos + OAuth)
- Edge computing en dispositius mèdics
- Integració amb sistemes sanitaris

## Notes inicials

Aquest apartat es construirà progressivament, a mesura que avancin:

- la PAC2 de Sistemes Distribuïts,
- el desenvolupament del TFG,
- i els experiments amb microserveis IA en entorns GitHub Codespaces.

Així es converteix la PAC en material de consulta permanent i en el marc
teòric pràctic del TFG.
