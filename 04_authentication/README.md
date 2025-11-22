# 04 – Autenticació en sistemes distribuïts

Aquesta secció recull els protocols i mecanismes d’autenticació utilitzats
en sistemes distribuïts moderns, amb especial atenció a entorns crítics
com els dispositius mèdics amb IA.

## Temes inclosos

- Protocol Needham–Schroeder (claus simètriques)
- Kerberos (tickets, KDC, autenticació robusta)
- OAuth 2.0 (autorització delegada)
- Autenticació basada en tokens (JWT, bearer tokens)
- Claus simètriques vs asimètriques
- Fluxos d’autorització
- Rejoc, atacs Man-in-the-Middle i mitigacions
- Models híbrids (Kerberos + OAuth, simètric + asimètric)

## Importància en sistemes mèdics distribuïts

Els dispositius mèdics intel·ligents necessiten:

- autenticació ràpida,
- segura,
- amb latència mínima,
- i tolerant a fallades.

La informació clínica és crítica, i l’autenticació s’ha d’adaptar a:
- connexions intermitents,
- dispositius offline,
- entorns on un servidor central pot no ser sempre accessible.

## Relació amb el TFG (ulleres mèdiques amb IA)

En el projecte de les ulleres IA apareixen diversos casos:

- autenticació entre ulleres i el servidor clínic,
- validació del metge que fa servir les ulleres,
- autorització per accedir a històries clíniques,
- microserveis IA que necessiten tokens segurs,
- infraestructures tipus “edge” amb connexió variable.

Els articles d’aquesta carpeta explicaran com cada protocol
soluciona (o no) aquests reptes i quines combinacions són més adequades.
