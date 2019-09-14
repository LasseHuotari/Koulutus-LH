# Datan valmistelu

Tässä vaiheessa poistamme datasta tarpeettoman kolumnin **CustomerID**.

1. Mene Watson Studiossa projektisi Assets sivulle.

2. Avaa Data Refinery painamalla datasetin actionin kohdalla löytyvää kolmea pistettä.

![](images/actions.png)

3. Vie hiiri **CustomerID** kolummnin nimen päälle, paina ilmestyvää kolmea pistettä ja valitse **Remove**

![](images/remove.png)

4. Nyt datasetti tulisi näyttää tältä

![](images/newset.png)

5. Paina seuraavaksi **Jobs** nappulaa ja valitse **Save and create a job**

![](images/jobs.png)

6. Anna jobille nimi, ja paina **Create and Run**

![](images/c&r.png)

7. Odota kunnas Status muuttuu **Completed** tilaan ja palaa sitten projektin asset sivulle, painamalla projektin nimeä vasemmalla ylhäällä.

![](images/completed.png)

8. Data Asset osioon on nyt tullut uusi datasetti, nimeltää **Mall_Customers.csv_shaped.csv**. Tämä data on nyt mallinnukselle valmisteltu datasetti.

![](images/shaped.png)
