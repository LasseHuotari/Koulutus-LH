# Mallin tuotteistaminen

Kuten mainittua tämän harjoituksen tarkoituksena on tehdä asiakkaalle rest-API rajapinta, jota pitkin he voivat kutsua malliaan. Tehdäksesi tämän harjoituksen tarvitse Watson Machine Learning instanssin. Saat tehtyä itsellesi kyseisen instanssin seuraamalla alla olevia ohjeita.

1. Mene osoitteeseen <a href="https://cloud.ibm.com" target="_blank">cloud.ibm.com</a> ja kirjaudu sisään.

2. Valitse oikealta ylhäältä **Catalog**

![](images/catalog.png)

3. Hae Watson Machine Learning, ja klikkaa palvelua listassa.

![](images/catalogwml.png)

4. Valitse Regioniksi Frankfurt, Varmista että Lite Plan on valittu ja nimeä instanssi

![](images/region.png)

![](images/plan.png)

![](images/name.png)

5. Paina create

![](images/create.png)

6. Avaa Watson Studio projektisi, ja avaa aikaisemmin luomasi modeler flow.

![](images/openflow.png)

7. Poista valitsemasi mallin ja type noden välissä oleva viiva klikkaamalla viivaa hiiren oikealla napilla ja painamalla **Delete**

![](images/delete.png)

8. Raahaa import valikon alta **User Input** node kanvakselle ja yhdistä se kultaisen malli noden vasempaan reunaan.

![](images/userinput.png)

9. Tupla klikkaa **User input** nodea ja paina **Define fields**

![](images/definefields.png)

10. paina **Add value**

![](images/addvalue.png)

11. Kirjoita **Fields** kohtaan **Age**, vaihda **Storage** arvo **Integer** muotoon, ja paina **Edit** kuvaketta.

![](images/valueedit.png)

12. Anna iäksi jokin esimerkki arvo, esimerkiksi **28**. Ja paina **OK**

![]images/assignvalue.png)

13. Toista sama Muuttujille_

* Annual Income (k$)
* Spending Score (1-100)
