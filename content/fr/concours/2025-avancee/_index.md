---
title : Classe avancée - 2025
description : Présentation du modèle d'avion de conception de drone autonome en vol VTOL et conventionnel pour la livraison et capture de charge utile en 2025, développé par l'Université d'Ottawa dans le cadre de la Classe avancée SAE.
---

{{< columns count=2 >}}
{{< column >}}
## Projet Longshot
### Plateforme d'avion de classe avancée SAE Aero uOttawa 2025 est conçue pour livrer et capturer des charges utiles de manière autonome via le VTOL et les vols conventionnels.

| Caractéristique | Valeur |
| --- | --- |
| Envergure | 1,2 m |
| Longueur | 0,97 m |
| Poids (vide) | `1,5 kg` |
{{< /column >}}

{{< model-viewer model="/models/advanced-2025.glb" poster="/models/advanced-2025.webp" camera-orbit="-137deg 80.15deg 2.514m" field-of-view="30" skybox-image="/models/stem.webp" skybox-height="0.3m" exposure="2">}}{{< /model-viewer >}}

{{< /columns >}}

{{< columns count=2 >}}

{{< column >}}


Le projet Longshot est construit autour d'un cadre modulaire en fibre de carbone et en imprimés 3D, qui comporte une envergure de 1,2 m avec un airfoil Clark-Y pour efficacité aérodynamique. Il est propulsé par trois unités T-Motor MN2806 légères et moteurs de soulèvement vectoriels à l'avant pour le vol vertical, offrant une bonne equilibrium entre la poussée et le poids sous les limites strictes de compétition. Le Pixhawk 6C est utilisé en tant que contrôleur de navigation et stabilité, soutenu par un Raspberry Pi CM4 pour la vision sur place et les positions GPS à précision RTK. La conception met l'accent sur la fiabilité, la modularité et la réparabilité, offrant une base solide pour le succès des missions dans la compétition de classe avancée SAE.
{{< /column >}}
{{< galimg src="img/adv-2025-longshot-glamour.jpg" caption="Projet Longshot, monté pour une photo de promotion" >}}
{{< /columns >}}

## Construction de la cellule
{{< columns count=2 >}}
{{< column >}}
Nous avons choisi une nouvelle technique de fabrication d'ailes : l'impression 3D. L'impression 3D des airfoils permet une grande souplesse dans la sélection de notre airfoil ainsi que la forme générale de l'aile. Nous avons utilisé ASA Aero, un fil filament qui a une densité extrêmement faible, ce qui rend nos ailes très légères pour leur taille. Les segments d'ailes imprimés 3D peuvent être glissés sur notre cadre en fibre de carbone, offrant une construction modulaire tout en permettant remplacement facile des sections d'ailes endommagées.
{{< /column >}}
{{< galimg src="img/adv-2025-spline.jpg" caption="Notre spline imprimé 3D collé à un barreau de fibre de carbone" >}}
{{< /columns >}}

## Construction de l'aile

{{< columns count=2 >}}

{{< column >}}

Nous avons choisi une nouvelle technique de fabrication d'ailes : l'impression 3D. L'impression 3D des airfoils permet une grande souplesse dans la sélection de notre airfoil ainsi que la forme générale de l'aile. Nous avons utilisé ASA Aero, un fil filament qui a une densité extrêmement faible, ce qui rend nos ailes très légères pour leur taille. Les segments d'ailes imprimés 3D peuvent être glissés sur notre cadre en fibre de carbone, offrant une construction modulaire tout en permettant l'easy remplacement des sections d'ailes endommagées.
{{< /column >}}

{{< galimg src="img/adv-2025-3d-printed-wing.jpg" caption="Notre aile imprimée 3D sur la plaque de pose" >}}

{{< /columns >}}

## Électroniques

{{< columns count=2 >}}
{{< column >}}
Nous avons construit un système électronique autour d'un Pixhawk 6c à partir de pièces détachées standard pour un prototype rapide et une connaissance qu'il était sûr que chaque module individuel avait été bien testé. Le Pixhawk 6c a été choisi pour son IO robuste, ses fonctionnalités et sa compatibilité avec le firmware [Ardupilot](https://ardupilot.org/). Ardupilot est capable d'effectuer des vols autonomes et contrôlés stabilisés en configuration horizontale et VTOL, effectuer un atterrissage précis à l'aide de données optiques et effectuer la transition VTOL à horizontale. Pour acquérir les données de précision pour le vol d'atterrissage réel-temps, nous utilisons un module Raspberry Pi CM4 avec une caméra monochrome globale à capteur CMO5017 pour suivre optiquement un marqueur fiduciaire sur la cargaison à environ 15Hz. Le contrôle et les télégrammes sont accomplis grâce à deux modules distincts : un module Sik de télégraphe et un module ERLS pour le contrôle manuel et l'armement. Le Pixhawk utilise un protocole numérique, DShot, pour la communication des escapements et les signaux PWM analogues pour les servomoteurs.
{{< /column >}}
<div>
{{< galimg src="img/adv-2025-electronics-plate.jpg" caption="Tout le matériel électronique branché" >}}
{{< spacer 50 >}}
{{< galimg src="img/adv-2025-ochin-and-camera.jpg" caption="le module CM4 de Raspberry Pi et la caméra Arducam OV2311 en tant que proof of concept" >}}
</div>
{{< /columns >}}

## Galerie de photos
{{< gallery >}}