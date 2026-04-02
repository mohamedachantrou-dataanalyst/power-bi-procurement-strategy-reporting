# Procurement Strategy Performance Analysis

**Secteur :** Purchasing · Supply Chain · Finance · Customer Service 

**Outils :** Power BI · DAX · Power Query · Excel

**Compétences :** Data Modeling · Data Analytics · Business Intelligence BI

---

## Contexte

Dans les entreprises industrielles, la stratégie d’achat joue un rôle clé dans la performance globale de l’organisation. La fiabilité des fournisseurs influence directement les opérations internes, les délais de livraison aux clients et la rentabilité.

Ce projet vise à analyser l’efficacité de la stratégie d’achat actuelle et à identifier les axes d’amélioration permettant d’optimiser la performance globale de l’entreprise.

---

## Objectif du projet

Répondre à la question stratégique suivante :

**Comment la stratégie d’achat actuelle influence-t-elle la performance globale et quelles actions concrètes peuvent être mises en place pour l’optimiser ?**

Pour cela, l’analyse est structurée autour de **trois axes majeurs :**

1. Fiabilité des fournisseurs
2. Impact sur les opérations internes
3. Impact business (satisfaction client et rentabilité)

---

## Modèle de données

Le projet repose sur 3 tables **dimensions** liées avec 2 tables **facts** **(Modéle en constellation)** :

**Fournisseurs**

``supplier_id``
``supplier_name``
``country``
``city``

**Commandes fournisseurs**

``order_id``
``product_id``
``supplier_id``
``order_date``
``expected_delivery_date``
``delivery_date``
``units_ordered``
``units_received``
``defect_units``
``unit_cost``
``transport_cost``
``penalty_cost``
``processing_time``
``manual_intervention``
``issues_count``
``rework_time``
``urgency_flag``

**Produits**

``product_id``
``product_name``
``category_id``

**Catégories d’achat**

``category_id``
``category_name``

**Commandes clients**

``order_id``
``order_date``
``expected_shipping_date``
``shipping_date``
``delay``
``delay_reason``

---

## Axes d'analyse

### 1️⃣ Fiabilité des fournisseurs

Évaluation de la performance logistique et qualité des fournisseurs :

Principaux KPI :

- % commandes livrées à temps (OTD)
- % commandes avec quantité manquante
- % commandes avec défauts qualité
- délai moyen de livraison
- performance par fournisseur
- comparaison avec les années précédentes

Objectif : identifier les fournisseurs présentant des risques pour la Supply Chain.

---

### 2️⃣ Impact sur les opérations internes

Analyse des conséquences des défaillances fournisseurs sur les opérations internes.

Principaux KPI :

- % commandes avec problèmes
- nombre moyen de problèmes par commande
- % commandes nécessitant du travail supplémentaire
- temps moyen de rework
- % commandes traitées en urgence
- % interventions manuelles

Objectif : mesurer les coûts opérationnels cachés générés par les fournisseurs.

---

### 3️⃣ Impact business

**Satisfaction client**

- % commandes clients impactées par les fournisseurs
- retard moyen dû aux fournisseurs
- comparaison avec les années précédentes

**Rentabilité**

- coût total d'achat
- pénalités fournisseurs
- répartition des pénalités par fournisseur

Objectif : mesurer l’impact direct des fournisseurs sur la performance financère et la satisfaction client.

---

## Structure du livrable

Le projet comprend : 

**1️⃣ Un rapport interactif structuré en plusieurs pages** :

- Page de navigation principale
- Fiabilité des fournisseurs
- Impact sur les opérations internes
- Impact sur la satisfaction client
- Impact sur la rentabilité
- Comparaison multicritères des fournisseurs
- Évaluation finale

**2️⃣ Un tableau de bord contenanant des insights clès** :



---

## Insights clés

Les analyses mettent en évidence plusieurs points critiques :

- Le taux de livraison à temps est **en dessous de la cible toute l’année**.
- **Zenith Corp** présente la plus mauvaise performance logistique (OTD de 71%).
- **Solaris Manufacturing** a le taux de défauts qualité le plus élevé (25%).
- **Quantum Industries** est le fournisseur avec le plus de quantités manquantes.
- Les problèmes fournisseurs entraînent :
  - une augmentation du travail supplémentaire
  - davantage d'interventions manuelles
  - une dégradation du taux de livraison client.

En 2025 :

- seulement **56% des commandes clients sont livrées à temps**
- **32% des retards sont liés aux fournisseurs**.

  Voir l'analyse complète !

---

## Recommandations stratégiques

L'analyse met en évidence plusieurs actions prioritaires.

### Amélioration de la fiabilité logistique

- Révision contractuelle avec **Zenith Corp** et **Nexus Supply**
- augmentation des stocks de sécurité sur les références critiques.

### Amélioration de la qualité

- audit qualité chez **Solaris Manufacturing**
- plan de correction pour **Quantum Industries**
- surveillance renforcée de **Infinity Components**.

### Réduction de l'impact opérationnel

- automatisation pour réduire les interventions manuelles
- actions correctives avec **Polaris Supply** et **Alpha Industries**.

### Rentabilité et satisfaction client

- maintien d'une politique de pénalités stricte
- transfert progressif du volume vers les fournisseurs les plus fiables.

  Voir l'ensemble des recommandations !

---

## Structure du repository

```
├── README.md
├── Data/
│    └── DataModel.png  
├── Analyse.txt
├── Recommandations.txt
├── Rapport/
│   └──ReportNavigationPage.png
│   └──SuppliersReliability.png
│   └──InternalOperationsImpact.png
│   └──CustomerSatisfactionImpact.png
│   └──ProfitabilityImpact.png
│   └──SuppliersComparison.png
│   └──FinalEvaluation.png
├── Dashboard/
    └── FinalDashboard.png
```

---

## Résultat
