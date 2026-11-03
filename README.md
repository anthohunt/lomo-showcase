> Showcase repository: the code and data of this project are private; this README describes it. / Dépôt vitrine : le code et les données de ce projet sont privés ; ce README le décrit.

# LoMo

A supply chain course where students design a European network, simulate it and compare a classic network with a Physical Internet network, on the web or in virtual reality.

## The problem

The Physical Internet proposes sharing warehouses, factories and carriers instead of each company owning its own. The idea stays abstract until you see it play out on costs, lead times and carbon. LoMo serves an engineering school for a master's module: students build two networks and measure the gap. Part of the group refused the headset, hence a complete web version.

## How it works

- The teacher prepares the scenario: cities, costs of warehouses, factories and trucks in euros and in carbon, products and bills of materials, demand per customer.
- The student places factories, warehouses and distribution centres on a map of 149 European cities and draws demand as curves (stable, seasonal, growing).
- They set decisions per site: trucks, production lines, storage, safety stock, logistics links.
- They first design a baseline network, then a Physical Internet version with hubs, open factories and warehouses, and independent carriers, among five modes.
- A simulation engine runs the network; a calculation service derives about thirty indicators from it (finance, service, stock, carbon).
- The two networks are shown side by side for comparison.

## What is built

On hold, nothing in production.

- A first version was used during the June 2026 course: online scenario builder, a fallback web page that reproduces the headset settings, export to the headset, import of results, Excel templates to work without a server.
- Bugs fixed along the way: a 28-city map exported instead of the 149-city one (actors lost, flat simulation), simultaneous saves overwriting each other (9 out of 10 lost before the fix).
- Since October, the course runs entirely inside the school's VR platform, web and Meta Quest headset, in multiplayer. The 15 steps of the build campaign were validated by an independent judge; 84 LoMo tests pass on the redesigned web page.
- A demo video is being shot: 7 sequences delivered out of 11.

## What is public

This showcase is public; the code, scenarios and course content stay private.

## Tech stack

- Unity, Meta Quest, Netcode for GameObjects
- Python for the scenario builder and Excel exports (openpyxl)
- Leaflet for the map
- Indicator service in Node.js and TypeScript
- Docker, Traefik

---

## Version française

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
