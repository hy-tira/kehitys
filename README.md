# Tietorakenteet ja algoritmit kehityssivu

## Yleiset asiat

* Kurssille tulisi lisätä videoita, niitä on toivottu paljon
* Tulisiko kurssilla olla luentoja? Niitä toivotaan mutta käytännössä harva käy luennoilla
* Paranna tiedotusta siitä, miten kurssille ilmoittaudutaan, milloin suoritukset tulevat ja mistä suorituksen pystyy näkemään (Opintopolusta)
* Paranna tiedotusta siitä, miten palautesysteemi toimii ja mitä käy jos ei saa linkkiä palautteen antamiseen

## Materiaali

* Enemmän kuvallisia esimerkkejä siitä miten verkkoalgoritmit toimivat
* Verkkoalgoritmien toteutukset ilman `float("inf")`-trikkiä, voisi toimia niin että ääretöntä etäisyyttä ei ole tallennettu
* Tuo esille, miten lyhimpiä polkuja etsitään suuntaamattomassa verkossa (nyt esimerkeissä vain suunnattuja)
* Tuo esille, että verkossa voi olla useita samanlaisia kaaria sekä kaari solmusta itseensä
* Pythonissa `set` ei säilytä alkioita suuruusjärjestyksessä vaikka voi näyttää siltä, esimerkki tästä materiaaliin

## Tehtävät

* Paranna luokkien testausta
  - Nyt voi olla paljon rivejä ja voi olla hankalaa nähdä riviä, jossa virhe esiintyy
  - Testeissä voi olla turhia rivejä (kuten peräkkäin samanlaisia hakuja ilman että välissä on muutoksia tietorakenteeseen)
  - Voisi olla hyvä aloittaa ensin lyhyistä testeistä (vain muutamia komentoja) ja edetä pidempiin testeihin
* Tuo esille kaikissa tehtävissä selkeästi, kuinka tehokas algoritmin tulisi olla (esim. “algoritmin tulee toimia tehokkaasti kun ruudukon koko on 100”)
* Voisiko testi kartoittaa ratkaisun suoritusaikaa, ja verrata sitä odotettuun? Tavoitteena hyödyllisempi palaute kuin "oli liian hidas". Esim. sovittamalla syötearvo→aika eri asteisiin polynomeihin, ja tutkimalla millä näistä korrelaatio oli paras. Ideaalinen palaute: "It looks like your function count has the running time complexity O(n²). Its running time complexity should be O(n log n) or better."
* Lisää tehtäviin esimerkkejä jotka selventävät tehtävänantoa
* Avoimissa tehtävissä monet vastaukset ovat huonoja/vääriä, pitäisi parantaa vastausten tarkastusta tai luopua näistä tehtävistä
* Avoimissa tehtävissä on myös opiskelijoille epäselvää, milloin voi menettää pisteen tehtävästä
* Olisiko tarvetta tietorakenteiden simulointiin?
* Paranna tiedotusta siitä, että joka viikko tulee ratkaista vähintään x tehtävää
* Binäärihakupuutehtävät mahdollista saada testeistä läpi koodilla jossa ei ole binääripuuta -> muuta testejä niin ettei tämä ole mahdollista (miten?)
* Tehtävä “Kaikki puut” (3103): monella googletettu (?) kaava jota ei ymmärretä
* Tehtävä “Tanssiaiset” (3207): epäselvää että molemmilla kampuksilla on n opiskelijaa. Voisi olla kuva, joka selventää tilannetta esimerkissä.
* Jos funktion palautusarvon tyyppi on väärä mutta vastaus muuten oikein, tämä tulisi näyttää selvästi
* Jos funktion pitäisi palauttaa tietorakenne, mutta on palautettu merkkijono, joka näyttää samalta kuin kyseisen tietorakenteen merkkijonoesitys, tämä tulisi näyttää selvästi
* Jos testattavalla funktiolla tai luokalla on sivuvaikutuksia, joiden johdosta se toimii oikein ensimmäisellä kutsulla mutta ei muiden testien jälkeen, tämä tulisi näyttää selvästi
  - Miten tämän voisi tarkastaa luotettavasti?
* Jos funktion parametri on lista tms. tietorakenne, tulisi varmistaa, että funktio ei muuta tietorakennetta
* Malliratkaisuja tulisi parantaa niin, että niitä olisi helpompaa ymmärtää (paremmin nimetyt muuttujat, kommentit, ei turhia trikkejä)
