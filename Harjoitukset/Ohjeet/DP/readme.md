# Datan valmistelu

Tässä vaiheessa poistamme datasta tarpeettoman kolumnin **CustomerID**.

1. Mene Watson Studiossa projektisi Assets sivulle.

2. Avaa Data Refinery painamalla datasetin actionin kohdalla löytyvää kolmea pistettä.

![](images/actions.png)

3. Vie hiiri **CustomerID** kolummnin nimen päälle, paina ilmestyvää kolmea pistettä ja valitse **Remove**

![](images/remove.png)

4. Nyt datasetti tulisi näyttää tältä

![](images/newset.png)

5. Seuraavaksi muokkaamme muuttujie nimeä. Korvaamme välilyönnit muuttujien nimestä ala viivalla, ja poistamme muuttujien selitteet muuttujien nimistä.

6. Vie hiiri **Annual Income (k$)** sarakkeen päälle ja valitse **kynä** ikoni.

![](images/renameaction.png)

7. Muokkaa sarakkeen nimi muotoon **Annual_Income**

![](images/annualincome.png)

8. Toista sama prosessi muuttujalle **Spending Score (1-100)** muuta se muotoon **Spending_Score**

![](images/spendingscore.png)

9. Paina seuraavaksi **Jobs** nappulaa ja valitse **Save and create a job**

![](images/jobs.png)

10. Anna jobille nimi, ja paina **Create and Run**

![](images/c&r.png)

11. Odota kunnas Status muuttuu **Completed** tilaan ja palaa sitten projektin asset sivulle, painamalla projektin nimeä vasemmalla ylhäällä.

![](images/completed.png)

12. Data Asset osioon on nyt tullut uusi datasetti, nimeltää **Mall_Customers.csv_shaped.csv**. Tämä data on nyt mallinnukselle valmisteltu datasetti.

![](images/shaped.png)
