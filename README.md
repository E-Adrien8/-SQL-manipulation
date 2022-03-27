# -SQL-manipulation
ecole de magie


INSERT INTO school (name, country, capacity) 
VALUES 
('Beauxbatons Academy of Magic', 'France', 550), 
('Castelobruxo', 'Brazil', 380), 
('Durmstrang Institute', 'Norway', 570), 
('Hogwarts School of Witchcraft and wizardry', 'United Kingdom', 450), 
('IIvermorny School of Witchcraft and Wizardry', 'USA', 300), 
('Koldovstoretz', 'Russia', 125), 
('Mahoutokoro School of Magic', 'Japan', 800), 
('Uagadou School of Magic', 'Uganda', 350);


UPDATE school SET country = 'Sweden' WHERE id = 3;

UPDATE school SET capacity = 700 WHERE id = 7;

DELETE FROM school WHERE name LIKE '%Magic%';


MariaDB [wild_db_quest]> select * from school;
+----+----------------------------------------------+----------+----------------+
| id | name                                         | capacity | country        |
+----+----------------------------------------------+----------+----------------+
|  2 | Castelobruxo                                 |      380 | Brazil         |
|  3 | Durmstrang Institute                         |      570 | Sweden         |
|  4 | Hogwarts School of Witchcraft and wizardry   |      450 | United Kingdom |
|  5 | IIvermorny School of Witchcraft and Wizardry |      300 | USA            |
|  6 | Koldovstoretz                                |      125 | Russia         |
+----+----------------------------------------------+----------+----------------+
5 rows in set (0.000 sec)

MariaDB [wild_db_quest]> 
