# Rapport de stage

To get inspired, go check this [link](https://github.com/gjoop/rapport-stage/blob/master/rapport.md).

# Introduction

Dans le cadre de stage obligatoire de fin d'année pour la formation délivrée par La Prépa des INPs, j'ai effectué un stage d'une durée d'un mois et demi dans l'entreprise SAP.

- [faire l'intro a la fin ]

# Cadre du stage

## Présentation de l'entreprise

### Généralités

SAP SE ou seulement SAP (SE signifiant "Societas Europaea" en latin) est une entreprise de droit européen dont le siège se trouve à Walldorf (Allemagne) qui conçoit et vend des logiciels. Ces logiciels sont principalement des outils permettant aux entreprises et aux institutions du monde entier de centraliser et analyser des données liées à leurs activités. SAP a été crée en 1972 par d'anciens employés d'IBM et s'appelait alors Systems Applications and Products in Data Processing.

Selon la liste Forbes de 2017 "The World's Biggest Public Companies", SAP est le premier producteur européen de logiciels et le troisième mondial derrière Microsoft (1) et Oracle (2). SAP est donc en concurrence directe avec Oracle et Microsoft, notamment sur son produit phare qui est le **progiciel de gestion intégrée**: SAP ERP.

![Forbes 2017 list of "The World's Biggest Public Companies"](Liste Forbes 2017.png)

Le terme **progiciel** est un mot-valise qui contracte "produit", "professionnel" et "logiciel". Il désigne une suite de logiciels applicatifs (qui sont directement utilisés pour accomplir une tâche), possédant de multiples fonctions et destinée à être utilisée par une large clientèle.

Un progiciel de gestion intégré **PGI**, ou son acronyme anglophone **ERP** (Enterprise Resource Planning), forme un **système d'information** (SI) pour une entreprise. Un **SI** est un ensemble organisé de ressources qui permet de collecter, stocker, traiter et distribuer de l'information. Pour un ERP, ce SI comporte un ensemble de modules fonctionnels, couvrant typiquement les achats, les stocks, la production, les ventes, la distribution, ainsi que les salaires, la comptabilité, les finances et la trésorerie. Tous les modules proviennent donc du même fournisseur (ici SAP) et travaillent sur une base de données unique (ici **HANA**, sur laquelle on reviendra plus tard).

Pour synthétiser, un logiciel ERP est un moyen d'intégrer les données de tous les départements d'une entreprise en un seul système accessible par tous, afin de faciliter les échanges d'informations. Il n'a donc pas de fonction d'analyse.

### Les Chiffres

![SAP Facts and Information](SAP facts and information.png)

Les produits SAP sont utilisés par de nombreuses entreprises dans le monde entier (plus de 388 000 clients dans plus de 180 pays).
Anciennement, SAP était perçu comme un produit que seul les grandes entreprises avaient les moyens de s'offrir. Or aujourd'hui, la plupart des clients sont des PMEs (environ 80%), cela vient du fait que SAP a adapté son offre à différents publiques.
Ce n'est pas pour autant que les grandes sociétés ne l'utilise plus. En effet, parmi les clients, on trouve par exemple 98% des marques possédant la valeur la plus élevée.
On peut constater que les revenus totaux IFRS de SAP, qui étaient de €23.76 milliards, sont en croissance (+9% au premier semestre de 2018). Et cela vient en grande partie de l'explosion de l'activité liée au Cloud (avec un taux de croissance de 31%).

SAP possède aussi plus de 100 centres d'innovations et de développement. Ces centres sont principalement situés en Allemagne, en France, en Irlande et aux USA.
Pour ce qui est de la France, le siège se situe au 35 rue d'Alsace dans la ville de Levallois-Perret. C'est donc dans cette tour de 20 étages que j'ai effectué mon stage du 30 Avril au 15 Juin 2018. On peut trouver dans cette tour des départements liés à plein de produits différents, mais aussi des départements liés aux ressources humaines, au service marketing ...
Cette organisation reflète une des philosophies phare de SAP qui est le **One SAP** sur laquelle on reviendra plus tard.

- [ talk about different centers + start up]

### Les Produits

Les produits SAP sont totalement intégrés, ce qui signifie qu'ils agissent comme un seul produit, avec donc une seule base de donnée et propose une mise à jour en temps réel des informations modifiées dans tous les modules affectés. Cela signifie aussi qu'il y a une totale traçabilité des opérations de gestion. Tous ces aspects permettent de mieux contrôler les aspects financiers, légaux et les ressources (manpower, machines, capacités de production).

On réduit souvent SAP au produit ERP et même à ce qu'on appelle "legacy ERP" ou l'ancien ERP, c'est à dire une suite logicielle "On-Premise" qui a divergée du produit original du fait de customisations importantes faites pas l'entreprise. C'est donc une suite que le vendeur ne supporte plus, qui coute cher à l'entreprise et qui est difficilement mis à jour. **On-Premise** signifie "sur site", cela veut donc dire que l'entreprise devait installer et mettre en place la suite SAP et ses bases de données sur ses propres serveurs. La maintenance devait alors être assurée par l'entreprise.

SAP a aujourd'hui pour but de changer cette image et a pour stratégie d'investir majoritairement dans le **Cloud** et les nouvelles technologies et en particulier ce qui touche aux analyses prédictives à l'aide d'intelligence artificielle.
Ainsi maintenant, SAP propose un large panel de produits dans plusieurs catégories:
* l'ERP (S/4HANA Cloud)
* Cloud et plateformes de données (Big Data, HANA)
* Achats et réseaux (fournisseurs et sources d'approvisionnement)
* Outils d'analyse (analyse prédictive, Business Intelligence BI)
* Client et commerce (marketing ...)
* IoT et chaîne logistique numérique (gestion d'objets connectés, gestion des stocks et fournisseur)
* Ressources humaines
* Gestion financière

La BI, aussi connue sous le nom d'informatique décisionnelle, représente l'ensemble des outils et méthodes permettant d'analyser puis de transmettre les informations pertinents aux managers d'entreprise (informations qui proviennent du système ERP) dans des formats adaptés: des dashboards contenant différents graphiques, des rapports etc...

Il y a aussi l'autre outils d'analyse: la **Predictive Analytics**. Alors que la BI n'a qu'un rôle d'analyse descriptive, la Predictive Analytics consiste à trouver et quantifier des motifs caché dans les données, ce qui permet après une analyse mathématique de construire des modèles qui permettront ensuite à partir de nouvelles données de prédire des résultats futurs.

SAP a pour objectif pour le deuxième semestre de 2018 de faire converger ces deux fonctions dans un seul produit, et ce dans le Cloud:

![SAP Convergence Strategy](BI-Convergence2.jpg)
[bi conv stratégie](https://news.sap.com/deeper-look-sap-strategy-bi-analytics/)

>SAP Analytics Cloud will be SAP’s primary solution for data discovery moving forward. New data discovery investments will be focused on SAP Analytics Cloud, where you can discover, analyze, plan, predict, and collaborate in one seamless experience that integrates with both on-premise and cloud-based data sources and applications.

C'est donc sur ce produit qui réunit la BI et l'analytique, qui se veut hybride (supporte à la fois les produits on-premise et les produits Cloud) et facile d'intégration, que j'ai travaillé.
Cette produit à pour vocation d'être intégré dnas la plateforme Cloud SAP: **SCP**

### Philosophies et stratégies

#### Stratégies

SAP oriente très fortement sa stratégie vers les nouvelles technologies qui sont:
* le Cloud: l'ensemble des services que l'on peut fournir via Internet
* l'IA, le Machine Learning et le Big Data: la possibilité, grâce à des algorithmes qui apprennent via des données, pour une machine de faire des choses intelligentes (prédictions, communication ...)
* IoT: Internet of Things: la gestion de l'ensemble des objets connectés
* la blockchain: un moyen rapide, sécurisé, transparent et stable pour communiquer et faire des transactions

On pourrait en fait regrouper toutes ces technologies dans le Cloud. On reverra plus en détail cette notion de Cloud.

#### Environnement



# cadre et organisation
-> présentation entreprise| environnement éco|logistique|ressources humaines(métiers) | communication/culture | boite rachetée | orga agile


# outils mission resultats

# Sources
[Progiciel](https://fr.wikipedia.org/wiki/Progiciel)

[PGI](https://fr.wikipedia.org/wiki/Progiciel_de_gestion_int%C3%A9gr%C3%A9)

[SAP Corporate Fact Sheet](https://www.sap.com/corporate/en/docs/download/2017/04/4666ecdd-b67c-0010-82c7-eda71af511fa.pdf)

[SAP Overview](https://searchsap.techtarget.com/definition/SAP)

[SAP products](https://www.sap.com/france/products.html)

[Comparative of ERP leaders](Clash-of-the-Titans-2017.pdf)

[Legacy ERP System](https://ercerp.wordpress.com/why-your-legacy-erp-system-needs-replacement/)

[From legacy ERP to S4/HANA](https://www.sap.com/france/products/erp/s4hana-erp.html#pdf-asset=6eec688c-927c-0010-82c7-eda71af511fa&page=2)

[SAP vs Oracle](https://www.quora.com/Why-is-SAP-generally-selected-over-Oracle-in-ERP)

[Business Intelligence](https://www.coheris.com/relation-client-data/solutions/analytics/la-business-intelligence-quest-ce-que-cest/)

[BI vs erp](https://www.sales-i.com/erp-vs-bi-the-difference)

[BI vs Predictive Analytics](http://olap.com/business-intelligence-versus-predictive-analytics/)

[SAP SE Purpose](https://www.sap.com/corporate/en/vision-purpose.html)

[SAP Blockchain](https://www.sap.com/products/leonardo/blockchain.html)

[roadmap sap 2018](https://blog.censio.fr/bi/roadmap-sap-analytics-2018/)

Conférence interne "ALL HANDS SAP LABS IN PARIS", 15 Mai 2018
