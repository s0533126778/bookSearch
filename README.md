# bookSearch
document:
+-----------+--------------+------+-----+---------+-------+
| Field     | Type         | Null | Key | Default | Extra |
+-----------+--------------+------+-----+---------+-------+
| book_name | varchar(120) | NO   | PRI | NULL    |       |
| subject   | varchar(120) | YES  |     | NULL    |       |
| author    | varchar(120) | YES  |     | NULL    |       |
| date      | date         | YES  |     | NULL    |       |
| location  | varchar(120) | YES  |     | NULL    |       |
| link      | blob         | NO   |     | NULL    |       |
+-----------+--------------+------+-----+---------+-------+
word:
+------------------+--------------+------+-----+---------+-------+
| Field            | Type         | Null | Key | Default | Extra |
+------------------+--------------+------+-----+---------+-------+
| sid              | int(120)     | NO   | PRI | NULL    |       |
| book_name        | varchar(120) | NO   | MUL | NULL    |       |
| word             | varchar(120) | NO   |     | NULL    |       |
| id_word_location | varchar(120) | YES  | MUL | NULL    |       |
+------------------+--------------+------+-----+---------+-------+
wordLocation:
+------------------+--------------+------+-----+---------+-------+
| Field            | Type         | Null | Key | Default | Extra |
+------------------+--------------+------+-----+---------+-------+
| id_word_location | varchar(120) | NO   | PRI | NULL    |       |
| page             | int(200)     | YES  |     | NULL    |       |
| line             | int(200)     | YES  |     | NULL    |       |
+------------------+--------------+------+-----+---------+-------+
