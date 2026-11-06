**English** · [Français](README.fr.md)

**Anthony Hunt** · [Project page on ingevision.cloud](https://ingevision.cloud/?lang=en&p=lomo) · [LinkedIn](https://www.linkedin.com/in/anthony-hunt-3948a9196) · [GitHub profile](https://github.com/anthohunt)

> Showcase repository: the code and data of this project are private; this README describes it.

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
