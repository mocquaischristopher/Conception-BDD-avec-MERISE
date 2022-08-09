# Conception-BDD-avec-MERISE
  
  > Votre mission est de concevoir la base de données d’une plateforme de formation en ligne nommée pire2pire.com à l'aide de la méthode MERISE.

## Définition acronyme MERISE

  > MERISE signifie "Méthode d'Etude et de Réalisation Informatique par les Sous-Ensembles ou les Systèmes d'Entreprise.

## Règles de gestion

  > Les règles de gestion sont les contraintes d'intégrité de ce que veut l'entreprise pour son application, ces règles doivent être respectées pour faire le MCD.

  1. Un module est caractérisé par un numéro en Sémantique Versionning, un intitulé, un objectif pédagogique, une durée (heures), un auteur (formateur)
  2. Une formation est caractérisé par un numéro en Sémantique Versionning, un nom
  3. Un formateur est caractérisé par un code unique (auto-incrément), un nom, un prénom
  4. Un apprenant est caractérisé par un code d'inscription unique (UUID), un nom, un prénom, una adresse, une date de naissance
  5. Un module contient un ou plusieurs contenus
  6. Un module contient un ou plusieurs tags
  7. Un module peut concerner un ou plusieurs formations
  8. Une formation est organisé par un seul formateur
  9. Une formation est terminé si tous les modules sont validés
  10. Un formateur peut être auteur d'un ou plusieurs modules
  11. Un apprenant peut s'inscrire à un ou plusieurs formations
  12. Un apprenant peut suivre un ou plusieurs modules
  13. Un apprenant peut valider lui-même un ou plusieurs modules
  14. Un apprenant est évaluer pour chaque module (un ou plusieurs) avec un état de fin de module (OK / KO)

## Dictionnaire de données

    | Nom | Signification | Type | Taille | Règles |
    |-----|---------------|------|--------|--------|
    |     |               |      |        |        |
    |     |               |      |        |        |
    |     |               |      |        |        |

  
## MCD (Modèle de Conception de Données)

  > Cela reprend toutes les données d'un système d'information. On se sert du dictionnaire de données ainsi que des règles de gestion afin de le crée.

## MLD (Modèle Logique de Données)

  >Le MLD est généré à partir du MCD, en transformant le MCD en un ensemble de tables.

## MPD (Modèle Physique de Données)

  > Le MPD est la continuité du MLD, c'est la transformation du MLD dans le format d'une base de données.

  > Le MPD peut être générer plusieurs fois grâce à un MLD afin de correspondre à une base de données spécifique : Oracle, MySQL, PostgreSQL, etc...

  > Cela donne au final le Script SQL.

## Script SQL de la base de données