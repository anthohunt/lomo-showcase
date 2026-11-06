[English](README.md) · **Français**

**Anthony Hunt** · [Fiche du projet sur ingevision.cloud](https://ingevision.cloud/?p=lomo) · [LinkedIn](https://www.linkedin.com/in/anthony-hunt-3948a9196) · [Profil GitHub](https://github.com/anthohunt)

> Dépôt vitrine : le code et les données de ce projet sont privés ; ce README le décrit.

# LoMo

Un cours de chaîne logistique où les étudiants conçoivent un réseau européen, le simulent et comparent un réseau classique à un réseau de l'Internet physique, sur le web ou en réalité virtuelle.

## Le problème

L'Internet physique propose de partager entrepôts, usines et transporteurs au lieu que chaque entreprise possède les siens. L'idée est abstraite tant qu'on ne la voit pas jouer sur des coûts, des délais et du carbone. LoMo sert à une école d'ingénieurs pour un module de master : les étudiants construisent deux réseaux et mesurent l'écart. Une partie du groupe refusait le casque, d'où une version web complète.

## Comment ça marche

- L'enseignant prépare le scénario : villes, coûts des entrepôts, usines et camions en euros et en carbone, produits et nomenclatures, demande par client.
- L'étudiant place ses usines, entrepôts et centres de distribution sur une carte de 149 villes d'Europe et dessine la demande par courbes (stable, saisonnière, en croissance).
- Il pose ses décisions par site : camions, lignes de production, stockage, stock de sécurité, liens logistiques.
- Il conçoit d'abord un réseau de base, puis une version Internet physique avec hubs, usines et entrepôts ouverts, et transporteurs indépendants, parmi cinq modes.
- Un moteur de simulation fait tourner le réseau ; un service de calcul en tire une trentaine d'indicateurs (finance, service, stock, carbone).
- Les deux réseaux s'affichent côte à côte pour être comparés.

## Ce qui est construit

En pause, rien en production.

- Une première version a servi pendant le cours de juin 2026 : constructeur de scénarios en ligne, page web de secours qui reproduit les réglages du casque, export vers le casque, import des résultats, modèles Excel pour travailler sans serveur.
- Bugs corrigés en route : une carte de 28 villes exportée à la place de celle de 149 (acteurs perdus, simulation plate), des sauvegardes simultanées qui s'écrasaient (9 sur 10 perdues avant correction).
- Depuis octobre, le cours se joue en entier dans la plateforme VR de l'école, web et casque Meta Quest, en multijoueur. Les 15 étapes de la campagne de construction ont été validées par un juge indépendant ; 84 tests LoMo passent sur la page web refondue.
- Une vidéo de démonstration est en tournage : 7 séquences livrées sur 11.

## Ce qui est public

Cette vitrine est publique ; le code, les scénarios et le contenu du cours restent privés.

## Pile technique

- Unity, Meta Quest, Netcode for GameObjects
- Python pour le constructeur de scénarios et les exports Excel (openpyxl)
- Leaflet pour la carte
- Service d'indicateurs en Node.js et TypeScript
- Docker, Traefik
