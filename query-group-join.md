## query to do:

### Group by:
1. Contare quanti iscritti ci sono stati ogni anno
```sql
SELECT YEAR(`students`.`enrolment_date`), COUNT(*)
FROM `students`
GROUP BY YEAR(`students`.`enrolment_date`);
```

2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio
```sql
SELECT `teachers`.`office_address`, COUNT(*)
FROM `teachers`
GROUP BY `teachers`.`office_address`;
```

3. Calcolare la media dei voti di ogni appello d'esame
```sql
SELECT `exams`.`id`, AVG(`exam_student`.`vote`) AS `average_vote`
FROM `exams`
JOIN `exam_student` ON `exam_student`.`exam_id` = `exams`.`id`
GROUP BY `exam_student`.`exam_id`;
```

4. Contare quanti corsi di laurea ci sono per ogni dipartimento
```sql

```

### Joins:
1. Selezionare tutti gli studenti iscritti al Corso di Laurea in Economia
```sql

```

2. Selezionare tutti i Corsi di Laurea Magistrale del Dipartimento di Neuroscienze
```sql

```

3. Selezionare tutti i corsi in cui insegna Fulvio Amato (id=44)
```sql

```

4. Selezionare tutti gli studenti con i dati relativi al corso di laurea a cui sono iscritti e il relativo dipartimento, in ordine alfabetico per cognome e nome
```sql

```

5. Selezionare tutti i corsi di laurea con i relativi corsi e insegnanti
```sql

```

6. Selezionare tutti i docenti che insegnano nel Dipartimento di Matematica (54)
```sql

```

7. BONUS: Selezionare per ogni studente il numero di tentativi sostenuti per ogni esame, stampando anche il voto massimo. Successivamente, filtrare i tentativi con voto minimo 18.
```sql

```