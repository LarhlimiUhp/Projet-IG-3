Guide de Réalisation de Dashboards sous Excel (ENCG Settat 2024-2025)

Résumé Exécutif

Ce document de synthèse détaille les principes méthodologiques et techniques pour la conception de tableaux de bord (dashboards) interactifs sous Excel, tels qu'enseignés dans le cadre du module « Informatique de Gestion — Tableur Avancé » à l'ENCG Settat (Université Hassan 1er).

Le dashboard est défini comme une interface visuelle centralisant les indicateurs clés de performance (KPI) pour faciliter le pilotage et la prise de décision. La méthodologie repose sur une structure de données rigoureuse (« Règle d'or »), l'utilisation systématique des Tableaux Excel dynamiques, et l'exploitation des Tableaux Croisés Dynamiques (TCD) comme moteur d'analyse. La réussite d'un dashboard dépend de l'équilibre entre la pertinence des indicateurs, l'interactivité (via les segments et chronologies) et une mise en page épurée respectant le principe « Moins c'est plus ».


--------------------------------------------------------------------------------


1. Fondamentaux et Typologie des Dashboards

Définition et Objectifs

Un dashboard est un outil visuel regroupant sur une vue unique les informations essentielles au pilotage d'une activité. Ses trois missions principales sont :

* Centraliser : Regrouper les informations en un lieu unique.
* Décider : Faciliter une prise de décision rapide par la visualisation.
* Suivre : Monitorer l'évolution des indicateurs dans le temps.

Catégories de Dashboards

Le support identifie quatre types distincts selon l'usage et l'audience :

Type	Audience	Objectif	Exemple
Stratégique	Direction Générale	Pilotage à long terme, KPI globaux	Balanced Scorecard (BSC)
Opérationnel	Managers intermédiaires	Suivi quotidien, indicateurs terrain	Suivi production / livraisons
Analytique	Data Analysts	Analyse approfondie, tendances	Ventes par région
Tactique	Responsables d'équipe	Objectifs trimestriels, moyen terme	Suivi budget trimestriel


--------------------------------------------------------------------------------


2. Préparation et Structuration des Données

La qualité du dashboard dépend exclusivement de la structure de la source. Le document énonce une Règle d'or : Une ligne correspond à un enregistrement, une colonne à un champ, et aucune cellule ne doit être fusionnée.

Critères de conformité des données

* En-têtes claires : Première ligne explicite, de préférence sans espaces ni accents.
* Types homogènes : Une colonne ne doit contenir qu'un seul type de données (dates, texte ou nombres).
* Absence de totaux : Ne jamais inclure de lignes de totaux dans la base source.
* Transformation en « Tableau Excel » (Ctrl+T) : Cette étape est cruciale car elle permet l'extension automatique des données, l'utilisation de références nommées (ex: =Ventes[CA]) et une actualisation simplifiée des TCD.


--------------------------------------------------------------------------------


3. Analyse via les Tableaux Croisés Dynamiques (TCD)

Le TCD est présenté comme l'outil essentiel pour synthétiser les données brutes.

Configuration et Fonctionnalités Avancées

* Les 4 Zones : Valeurs (calculs numériques), Lignes (axe vertical), Colonnes (axe horizontal) et Filtres (segmentation globale).
* Champs Calculés : Permettent de créer de nouveaux indicateurs basés sur des formules (ex: Marge % = (CA - Coût) / CA).
* Groupement par Date : Excel permet de passer d'une granularité journalière à une vision par mois, trimestre ou année par un simple clic droit.
* Conseil de maintenance : Il est recommandé de créer un TCD distinct pour chaque indicateur afin de garantir l'indépendance des graphiques.


--------------------------------------------------------------------------------


4. Visualisation de Données et Interactivité

Choix du Graphique Croisé Dynamique (GCD)

Le support préconise des types de graphiques spécifiques selon la nature de l'information :

Type de Graphique	Usage Recommandé
Histogramme / Barres	Comparer des catégories (ex: Ventes par produit)
Courbe / Ligne	Tendances dans le temps (ex: Évolution CA mensuel)
Secteurs / Anneau	Répartition des parts (limité à 5-6 parts maximum)
Aire	Cumul des ventes, suivi des objectifs
Jauge / Compteur	Indicateur unique, taux de réussite



--------------------------------------------------------------------------------


5. Mise en Forme Conditionnelle (MFC) et Finalisation

Règles Visuelles (Alertes)

La MFC permet de colorier automatiquement les cellules selon des seuils définis :

* Vert : Objectif atteint (≥ 100%).
* Orange : Proche de l'objectif (80-99%).
* Rouge : Alerte (< 80%).
* Outils supplémentaires : Barres de données, nuances de couleurs (cartes thermiques) et jeux d'icônes (flèches, feux tricolores).

Structure Recommandée du Classeur

Pour un aspect professionnel et une maintenance aisée, le classeur doit être organisé en feuilles distinctes :

1. DONNÉES : Base brute structurée en Tableau Excel.
2. CALCULS : TCD et tables intermédiaires (masquée à l'utilisateur final).
3. DASHBOARD : Vue finale soignée, sans formules visibles.
4. PARAMS : Configuration des seuils, objectifs et listes de référence.


--------------------------------------------------------------------------------


6. Pratique : Étude de Cas en Distribution

Dans le cadre du cours, un exercice d'application est proposé pour un contrôleur de gestion au Maroc (contexte incluant des entités comme OCP, Attijariwafa Bank ou Maroc Telecom).

Indicateurs à produire pour le suivi des ventes :

* KPIs Flash : CA Total, Marge brute (%), Nombre de commandes.
* Analyses Temporelles : Évolution mensuelle du CA.
* Analyses Segmentées : CA par région, Top 5 produits (barres horizontales), répartition par catégorie.


--------------------------------------------------------------------------------


7. Règles d'Or pour un Dashboard Professionnel

* Lois de Design : Limiter à 6-8 indicateurs maximum. Utiliser une palette de 2-3 couleurs et une police unique.
* Maintenance : Utiliser le bouton « Actualiser tout » (Ctrl+Alt+F5) pour intégrer les nouvelles données.
* Sécurité : Masquer le quadrillage, les en-têtes de lignes/colonnes et protéger la feuille pour que l'utilisateur ne puisse interagir qu'avec les segments.
* Adaptabilité : Tester sur différentes résolutions et prévoir une version imprimable (Format A3).
* Documentation : Inclure une feuille "README" pour expliquer les sources et la structure.
