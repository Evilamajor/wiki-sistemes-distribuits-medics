# 03 – Gestió de la concurrència

Aquesta secció recull els mecanismes que permeten controlar l’accés concurrent
a dades distribuïdes, tant en entorns eventualment consistents com en sistemes
de baixa latència com els dispositius mèdics amb IA.

## Temes inclosos

- Concurrència optimista
- Concurrència pessimista
- Model de lectura/escriptura
- Resolució de conflictes
- Detecció de concurrència (Lamport, vector clocks)
- CRDT (Conflict-free Replicated Data Types)
- Escriptura local i reconciliació posterior (Bayou/Coda)
- Implicacions en sistemes de salut i dispositius mèdics

## Relació amb el TFG (ulleres mèdiques amb IA)

Les ulleres IA poden generar conflictes quan:
- dues ulleres creen anotacions a la vegada,
- un microservei IA i un professional fan operacions simultànies,
- el sistema està offline i cal reconciliar dades posteriorment.

Aquest directori contindrà els articles que expliquen aquests conceptes
amb exemples aplicats al projecte del TFG.
