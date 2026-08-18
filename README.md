# Univers profond — simulateur 3D du système solaire

Simulation web 3D (Three.js) du système solaire et de son environnement galactique,
entièrement contenue dans un seul fichier HTML — aucune installation, il suffit
d'ouvrir `index.html` dans un navigateur.

## Contenu

- **Système solaire** : 8 planètes texturées, lunes, anneaux, ombres portées, rotations et orbites réalistes
- **Ceinture d'astéroïdes** (Mars → Jupiter) : plus de 55 000 points de poussière et de gravats + 294 rochers 3D sur orbites képlériennes, avec Cérès, Vesta et Pallas
- **Ceinture de météoroïdes** (Terre → Mars) : bande de poussière zodiacale et météoroïdes en rotation
- **Ceinture de Kuiper** : ~100 000 objets répartis en 7 couches, disque dispersé, amas résonants, 380 rochers glacés en orbite, Pluton/Charon, Makémaké, Hauméa
- **Confins** : héliopause, nuage d'Oort, comètes nommées sur orbites elliptiques
- **Soleil** : photosphère animée par shader (granulation, taches), chromosphère et couronne à streamers façon éclipse
- **Ciel profond** : Voie lactée, Andromède, M13, amas globulaires, Sagittarius A* et Cygnus X-1
- **SkyMap** : planétarium hors-ligne (700+ étoiles, NGC/IC, constellations) avec boussole mobile

## Commandes

- Souris / doigts : orbite, zoom, déplacement
- Curseur **☀️ Soleil** : pilote toute l'illumination (lumière solaire, ambiance, exposition, éclat de la couronne et des ceintures)
- Curseurs **🌙 Orbite lune** et **Vitesse** : rythme de la simulation
- **H** ou le bouton **☰ Menu** : masquer / afficher le panneau flottant
- **🎬 Visite guidée** : tour commenté du système solaire

## Technique

Three.js 0.160 via importmap CDN, EffectComposer (bloom, lensflare), shaders GLSL
personnalisés pour le Soleil, la Terre de nuit et les disques d'accrétion. Toutes les
textures sont générées procéduralement sur canvas — aucun asset externe.
