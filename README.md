# Floating 3D Model Scene (Three.js + GSAP + ScrollTrigger)

Ce projet recrée une scène 3D interactive avec **Three.js**, **GSAP ScrollTrigger**, **Lenis** pour le smooth scroll, et des **animations synchronisées avec le scroll**.  
Inspiré du tutoriel :  
🎥 [Floating 3D Scene + ScrollTrigger Tutorial (YouTube)](https://youtu.be/rbIbvw6c53k?si=hSqoJ-jsmh7Dcmin)

## Functionaliteiten
- 3D model geladen met GLTFLoader
- Smooth scroll via Lenis
- ScrollTrigger om:
  - backgrounds te veranderen
  - animaties te starten op scroll
  - model te laten verdwijnen / draaien / floaten
- GSAP animaties (scale, rotation, float)
- Transparant canvas bovenop een CSS background
- Dynamisch aanpassen van achtergrondbeelden
- Audio trigger bij scan (optioneel)

## Gebruikte code en bronnen

1. `import * as THREE from "three";`  
   → Basis van de 3D scene, camera, renderer, materials  
   🔗 https://threejs.org/docs/

2. `import { GLTFLoader } from "three-stdlib";`  
   → Laadt het `.glb` 3D model  
   🔗 https://threejs.org/docs/#examples/en/loaders/GLTFLoader

3. `const renderer = new THREE.WebGLRenderer({ alpha: true });`  
   → Transparant canvas zodat je CSS background erdoor komt  
   🔗 https://threejs.org/docs/#api/en/renderers/WebGLRenderer

4. `ScrollTrigger.create({ ... })`  
   → Activeert animaties en background wissels op scroll  
   🔗 https://gsap.com/docs/v3/Plugins/ScrollTrigger/

5. `gsap.to(model.scale, { ... })`  
   → GSAP animatie voor het laten verschijnen of verdwijnen van het model  
   🔗 https://gsap.com/docs/v3/

6. `camera.aspect = window.innerWidth / window.innerHeight;`  
   → Zorgt dat camera correct schaalt bij venstergrootte  
   🔗 https://threejs.org/docs/#api/en/cameras/PerspectiveCamera

7. 🎥 YouTube Tutorial (origineel)  
    🔗 https://youtu.be/rbIbvw6c53k?si=hSqoJ-jsmh7Dcmin


