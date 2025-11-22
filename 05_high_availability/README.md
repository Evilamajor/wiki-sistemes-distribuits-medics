# 05 – Alta disponibilitat i tolerància a fallades

Aquesta secció recull els models i protocols que permeten que un sistema distribuït
continuï funcionant fins i tot quan hi ha fallades, latència o desconnexions
intermitents. És un aspecte clau per a dispositius mèdics, on la disponibilitat
pot tenir impacte directe en la seguretat del pacient.

## Temes inclosos

- Alta disponibilitat (HA) en sistemes distribuïts
- Replicació de dades
- Tolerància a fallades
- Sistemes basats en gossip
- Protocol Bayou (escriptura local + reconciliació)
- Sistema Coda (desconnexió i reintegració)
- Consistència eventual
- Quorum (lectures i escriptures)
- Replis lògics vs replis físics
- Failover / failback
- Models CAP aplicats a entorns clínics

## Importància en dispositius mèdics amb IA

En entorns sanitaris:
- la xarxa no sempre és perfecta,
- hi poden haver desconnexions temporals,
- els dispositius poden estar en moviment (ulleres, tauletes, monitors portàtils),
- la latència ha de ser mínima,
- i les dades han de ser fiables.

Els mecanismes HA permeten:
- continuar operant fins i tot sense servidor,
- sincronitzar-se quan torna la connexió,
- evitar la pèrdua d’informació clínica,
- mantenir els microserveis IA disponibles.

## Relació amb el TFG (ulleres mèdiques amb IA)

Les ulleres IA funcionen en un entorn distribuït amb:
- diversos dispositius,
- microserveis,
- servidors clínics,
- connexions irregulars.

Per això necessiten:
- replicació de logs clínics,
- sincronització posterior (Coda/Bayou),
- consistència eventual controlada,
- mecanismes de reconciliació semàntica,
- un lideratge lleuger (Raft) per coordinar l’estat global.

Els articles d’aquest directori explicaran amb detall tots aquests conceptes
i com aplicar-los al disseny final de la plataforma del TFG.
