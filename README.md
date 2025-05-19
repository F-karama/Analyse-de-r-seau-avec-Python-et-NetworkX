# Analyse d’impact d’une intervention sur les collaborations scientifiques

Ce projet a été réalisé lors de l’UE **« Analyse des réseaux »** de M1 IREF, en collaboration avec Barkiré Douramane Moussa. Il vise à étudier l’effet d’une intervention politique destinée à encourager les collaborations scientifiques entre chercheurs. Un réseau de scientifiques a été observé **avant** et **après** cette intervention afin d’en évaluer l’efficacité.


## Description des données

Nous disposons de deux fichiers CSV reliés par un identifiant individuel (`id`) :

1. **nodes.csv** – Informations invariables dans le temps sur chaque agent

   * `id` : identifiant de l’agent
   * `coord` : vaut 1 si la personne est coordinatrice du cluster (parfois non listée)
   * `core`  : vaut 1 si la personne a été identifiée, avant traitement, comme membre « core » du cluster (dans l’espace d’expertise)
   * `gender`: vaut 1 pour les femmes

2. **edges.csv** – Informations variant dans le temps sur les dyades

   * `source`, `target` : identifiants des deux agents formant la dyade
   * `pre_link`  : collaboration scientifique active avant l’intervention
   * `post_link` : collaboration scientifique active après l’intervention

> NB : Toutes les collaborations sont **non orientées** : chaque dyade apparaît deux fois (une fois dans chaque sens).



## Objectifs de l’analyse

1. **Étudier la structure et l’évolution du réseau**

   * Mesures statistiques (densité, centralité, distribution des degrés…)
   * Visualisation des graphes avant et après intervention

2. **Explorer l’influence des attributs “core” et “genre”**

   * Les femmes forment-elles des réseaux plus ou moins denses que les hommes ?
   * Sont-elles plus ou moins centrales ?
   * Comment évoluent leurs collaborations après l’intervention par rapport aux hommes ?
   * Y a-t-il des communautés ou de l’homophilie avant/après le traitement ?
   * L’appartenance au “core” module-t-elle ces évolutions ?

