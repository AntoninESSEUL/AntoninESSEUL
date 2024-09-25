# Commandes de base SQL

## Gestion de bases de données

- `CREATE DATABASE nom_base;` : Crée une nouvelle base de données.
- `DROP DATABASE nom_base;` : Supprime une base de données.
- `USE nom_base;` : Sélectionne une base de données pour l’utiliser.
- `SHOW DATABASES;` : Liste toutes les bases de données disponibles.
- `SHOW TABLES;` : Liste toutes les tables dans la base de données sélectionnée.

## Gestion des tables

- `CREATE TABLE nom_table (colonne1 TYPE, colonne2 TYPE, ...);` : Crée une nouvelle table avec des colonnes définies.
- `DROP TABLE nom_table;` : Supprime une table.
- `ALTER TABLE nom_table ADD colonne TYPE;` : Ajoute une nouvelle colonne à une table.
- `ALTER TABLE nom_table DROP COLUMN colonne;` : Supprime une colonne d’une table.
- `ALTER TABLE nom_table RENAME TO nouveau_nom_table;` : Renomme une table.
- `DESCRIBE nom_table;` : Affiche la structure d'une table.

## Insertion de données

- `INSERT INTO nom_table (colonne1, colonne2, ...) VALUES (valeur1, valeur2, ...);` : Insère de nouvelles données dans une table.
- `INSERT INTO nom_table VALUES (valeur1, valeur2, ...);` : Insère des données dans toutes les colonnes dans l'ordre défini par la table.

## Mise à jour et suppression de données

- `UPDATE nom_table SET colonne1 = 'valeur' WHERE condition;` : Met à jour des données dans une table.
- `DELETE FROM nom_table WHERE condition;` : Supprime des enregistrements d'une table.
- `TRUNCATE TABLE nom_table;` : Supprime tous les enregistrements d'une table sans supprimer la table.

## Requêtes de sélection de données

- `SELECT colonne1, colonne2 FROM nom_table;` : Sélectionne des colonnes spécifiques d'une table.
- `SELECT * FROM nom_table;` : Sélectionne toutes les colonnes d'une table.
- `SELECT colonne1, colonne2 FROM nom_table WHERE condition;` : Sélectionne des colonnes avec une condition.
- `SELECT colonne1, COUNT(*) FROM nom_table GROUP BY colonne1;` : Groupe les résultats par une colonne et compte le nombre d'occurrences.
- `SELECT colonne1, colonne2 FROM nom_table ORDER BY colonne1 ASC;` : Trie les résultats par ordre croissant (ASC) ou décroissant (DESC).
- `SELECT DISTINCT colonne FROM nom_table;` : Sélectionne uniquement les valeurs distinctes dans une colonne.

## Clauses avancées

- `WHERE` : Filtre les résultats selon une condition.
  - Exemples : 
    - `WHERE colonne = 'valeur'`
    - `WHERE colonne > 100`
    - `WHERE colonne LIKE 'mot%'` : Recherche de correspondance partielle.
- `AND` / `OR` : Combine plusieurs conditions.
  - Exemple : `WHERE colonne1 = 'valeur1' AND colonne2 = 'valeur2'`
- `BETWEEN valeur1 AND valeur2` : Sélectionne des résultats compris entre deux valeurs.
- `IN (valeur1, valeur2, ...)` : Filtre les résultats appartenant à une liste de valeurs.
- `IS NULL` / `IS NOT NULL` : Filtre les résultats avec ou sans valeur nulle.

## Jointures (Joins)

- `INNER JOIN` : Retourne les enregistrements correspondants dans les deux tables.
  - Ex : `SELECT * FROM table1 INNER JOIN table2 ON table1.colonne = table2.colonne;`
- `LEFT JOIN` : Retourne tous les enregistrements de la première table et les correspondances de la deuxième table.
- `RIGHT JOIN` : Retourne tous les enregistrements de la deuxième table et les correspondances de la première table.
- `FULL JOIN` : Retourne tous les enregistrements lorsqu'il y a une correspondance dans une des tables.

## Fonctions d'agrégation

- `COUNT(colonne)` : Compte le nombre d'enregistrements.
- `SUM(colonne)` : Retourne la somme des valeurs dans une colonne.
- `AVG(colonne)` : Retourne la moyenne des valeurs dans une colonne.
- `MAX(colonne)` : Retourne la valeur maximale dans une colonne.
- `MIN(colonne)` : Retourne la valeur minimale dans une colonne.
