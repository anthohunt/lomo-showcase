[English](README.md) · **Français**

# LoMo

**Les étudiants conçoivent un réseau logistique européen, le simulent, puis le refont avec les options de l'Internet physique et mesurent l'écart.** Un module de cours de la plateforme HITeC, joué ensemble sur ordinateur, téléphone ou casque Meta Quest.

[![La carte du réseau de départ, un centre de traitement ouvert à Madrid, un calcul de 150 jours et ses quatre résultats, puis le passage au transport hyperconnecté vu sur un téléphone (cliquer pour la vidéo complète)](docs/demo.gif)](https://drive.google.com/file/d/1oU39vlcpxEfFu0RXz3ERBBnLPYjn2RT0/view)

*La carte, un nouveau centre de traitement, un calcul de 150 jours, puis le transport hyperconnecté vu sur un téléphone. [Vidéo complète (2:17)](https://drive.google.com/file/d/1oU39vlcpxEfFu0RXz3ERBBnLPYjn2RT0/view)*

## Ce qu'on fait avec

- **Salle.** Le professeur ouvre une salle et charge un scénario : fournisseurs, une usine, un centre de distribution, des clients dans toute l'Europe, une année en trois saisons.
- **Places.** Chaque élève prend une installation, depuis un navigateur, un téléphone ou le casque. Un changement fait n'importe où s'affiche chez tous.
- **Décisions.** Les élèves ouvrent des centres de traitement sur la carte (taille S, M ou L), puis règlent étagères, camions et lignes de production saison par saison. Une liste bloque le calcul tant qu'il manque quelque chose.
- **Simulation.** Le professeur lance 150 jours de livraisons. Les résultats tiennent en quatre familles (efficience, carbone, service, coût), puis installation par installation.
- **Cinq réglages.** Le réseau de base, puis quatre réglages de l'Internet physique : transport hyperconnecté, centres de distribution et de traitement ouverts, fabrication distribuée, usines ouvertes. Chacun est comparé au réseau de base.

## Architecture

![Architecture de LoMo : les navigateurs passent par le site HITeC, les casques par un moteur de salle en Netcode ; le moteur de salle envoie le réseau au service d'indicateurs, qui fait simuler les livraisons par le moteur de simulation](docs/architecture.fr.svg)

## État

- **Juin 2026.** Première version utilisée en cours. Les étudiants ont refusé le casque : le cours a été refait d'abord pour le web, casque en option.
- **Octobre 2026.** Deuxième version dans HITeC : 15 étapes, chacune validée par un relecteur indépendant.
- **Aujourd'hui.** En pause depuis le 1er novembre 2026, pas en production. L'instance de test du serveur de l'école (Docker, réseau de l'école seulement) est arrêtée.
- **Pile.** Unity (appli du casque, un serveur dédié par salle, Netcode for GameObjects), Node.js et TypeScript, Python avec FastAPI et Redis, nginx.

---

**Anthony Hunt** · [ingevision.cloud](https://ingevision.cloud/?p=lomo) · [LinkedIn](https://www.linkedin.com/in/anthony-hunt-3948a9196) · [GitHub](https://github.com/anthohunt)

Le code, les scénarios et le contenu du cours restent privés. La vidéo utilise des comptes de démonstration et un scénario de test.
