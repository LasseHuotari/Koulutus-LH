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

![](images/assignvalue.png)

13. Toista sama Muuttujille

* Annual_Income
* Spending_Score

14. Lopuksi pitäisi näyttää tältä, asettamasi esimerkki arvot tietenkin voivat vaihdella. Paina **OK** ja sen jälkeen **Save**

![](images/userinputready.png)

15. Vie hiiri **Table** Noden päälle, ja paina kolmea pistettä, jonka jälkeen paina **Run**

![](images/tablerun.png)

16. Tupla klikkaa avautuvasta **Outputs** valikosta **Table (4 fields, 1 recors)** kuvaketta.

![](images/prediction.png)

17. Nyt näät itse ennusteen tuloksen. Sarake $KM-K-Means kertoo mihin segmenttiin kyseinen asiakas ennusteen mukaan kuuluisi. Oma tuloksesi saattaa poiketa alla näkyvästä, koska saatoit valita eri määrän klustereita omaan malliisi, mutta taulukon rakenne pitäisi olla sama.

![](images/predictiontable.png)

18. Palaa kanvakselle painamalla flow nimeä.

![](images/back2canvas.png)

19. Seuraavaksi vie hiiri jälleen **Table** noden päälle ja valitse kolme pistettä, ja paina **Save branch as a model**

![](images/savemodel.png)

20. Anna mallillesi nimi, ja paina **Save**

![](images/modelname.png)

21. Kun saat vahvistuksen että malli on tallentunut ja olet palannut takaisin kavakselle, palaa Projektin Asset sivulle painamalla projektin nimeä

![](images/back2project.png)

22. Näät tallennetun mallin **Models** kohdassa. Paina Mallin nimeä.

![](images/projectmodel.png)

23. Valitse Deployment välilehti ja paina **Add deployment**

![](images/depl.png)

24. Anna deploymentille nime, ja paina **Save**

![](images/deplname.png)

25. Odota kunnes **Status** on **DEPLOY_SUCCESS** ja paina tämän jälkeen deploymentin nimestä.

![](images/deplsuccess.png)

26. Mene **Test** välilehdelle, syötä seuraava koodi **Enter input data** kenttään ja paina **Predict**

~~~
{"fields": ["Age","Annual_Income","Spending_Score"], "values": [[28,20,80]]}
~~~

![](images/predict.png)

27. Jos sait edellisen kaltaisen näkymän niin rest-API toimii, ja olet tuotteistanut mallisi tuotantoon. Jos haluat itse tehdä sovelluksen mallista, löydät tarkat kutsuohjeet eri koodikielillä **Implementation** välilehdeltä.
