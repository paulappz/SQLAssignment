# SQLAssignment

```SQL

1.	/* SQL Query for creating table named 'award'*/

CREATE TABLE IF NOT EXISTS `awards`.`award`(
  `award_id` INT NOT NULL AUTO_INCREMENT,
  `title` TEXT NOT NULL,
  `description` TEXT NOT NULL,
  PRIMARY KEY(`award_id`)
) ENGINE = InnoDB;



2.	/* SQL Query for inserting into table named 'award'*/

INSERT
INTO
  `award`(`award_id`,
  `title`,
  `description`)
VALUES(
  '1',
  'Best Female Author of the year',
  'This Award is given to the best author of the year in the female category'
);


3.	/* SQL Query for retrieving all infomation in the table named 'award'*/

SELECT
  *
FROM
  'award'


4.	/* SQL Query for updating a particuar row in table named 'award'*/

UPDATE
  `award`
SET
  `title` = 'Best Male Author of the year',
  `description` = 'This Award is given to the best author of the year in the male category'
WHERE
  `award_id` = '1'


  5.	/* SQL Query for deleting a particuar row in table named 'award'*/

DELETE
FROM
  `award`
WHERE
  `award_id` = '1'

