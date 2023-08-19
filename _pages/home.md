---
title: ""
layout: single
permalink: /
author_profile: true
classes: wide
header:
  overlay_color: "#000"
  overlay_filter: "0.6"
#   overlay_image: /images/particles.jpg
excerpt: "Stage Télécom Paris - ATIAM"
---

## Introduction
<html>
<div style="text-align: justify">
<p>
Ce projet est le résultat d'un stage de recherche de 6 mois effectué au laboratoire LTCI de <a href="https://www.telecom-paris.fr/fr/recherche/laboratoires/laboratoire-traitement-et-communication-de-linformation-ltci" target="_blank" rel="noopener noreferrer">Télécom Paris</a>, dans l'équipe <a href="https://adasp.telecom-paris.fr/" target="_blank" rel="noopener noreferrer">ADASP</a> et sous la supervision de Gaël Richard.
</p>

<p>
L'objectif du projet est de séparer les 4 voix : Soprano, Alto, Ténor et Basse d'un enregistrement de chant choral. Cette technique est appelée Séparation de Sources, et dans notre cas, elle est réalisée à partir de modèle d'apprentissage profond non supervisé. C'est à dire, qu'il n'y a pas besoin des sources isolées pour l'entrainement.
</p>
</div>
</html>

## Résumé

<html>
<div style="text-align: justify">
<p>
Dans le domaine de la séparation de sources musicales, les algorithmes les plus performants sont généralement ceux basés sur des méthodes d’apprentissage profond supervisé. Cependant, ces approches nécessitent la connaissance des sources isolées pour l’entrainement, ce qui peut être compliqué à obtenir en pratique. Pour surmonter cette limitation, l’utilisation de méthodes non supervisées est alors requise et s’exprime sous la forme d’algorithmes basés sur des connaissances a priori. Dans notre travail, nous proposons d’approfondir un modèle d’apprentissage profond de séparation de sources musicales non supervisé [39], basé sur des modèles source-filtre paramétriques différentiables. Celui-ci utilise en tant
que connaissance a priori les fréquences fondamentales de chaque source, dont nous souhaitons intégrer l’estimation à l’intérieur du modèle afin qu’elle soit apprise conjointement avec les autres paramètres. Nous avons donc implémenté une architecture de réseau de neurones, basée sur des modèles pré-entrainés, permettant d’apprendre simultanément la tâche de synthèse initiale et la tâche d’estimation de fréquences fondamentales multiples. Dans le cadre de cette approche, nous proposons également différentes méthodes pour une extraction de contours différentiable, et montrons que cela permet d’entrainer les deux tâches simultanément. Enfin, nous évaluons notre architecture selon plusieurs méthodes
d’entrainement, et démontrons sa capacité à obtenir des performances satisfaisantes dans certaines configurations. Des expériences complémentaires ont également permis d’améliorer le modèle d’origine en réduisant significativement son temps d’entrainement et le traitement des données.
</p>

</div>
</html>

*Mots clés: Séparation de Sources Musicales, Estimations de fréquences fondamentales multiples, Assignement de voix, Apprentissage non supervisé, Architecture hybride*
