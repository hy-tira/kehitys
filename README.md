# Tietorakenteet ja algoritmit kehityssivu

## Yleiset asiat

* Kurssille tulisi lisätä videoita, niitä on toivottu paljon
* Paranna tiedotusta siitä, miten palautesysteemi toimii ja mitä käy jos ei saa linkkiä palautteen antamiseen
* Moni käyttää tekoälyä ja tätä on vaikeaa valvoa, tulisiko kurssin formaattia muuttaa?
* Kurssia pidetään (liian?) vaikeana ja työläänä, toisaalta viikon alkupään tehtävät voivat olla liian helppoja
  - Kurssin saa (liian?) helposti läpi mutta korkeampia arvosanoja on (liian?) vaikeaa saada
  - Liian jyrkkä kasvu tehtävien vaikeudessa?
* "Esitietovaatimuksista voisi mielestäni hyvin jättää pois JYM-kurssin (ja melko lailla kaikki muutkin matematiikan kurssit) – ei niitä oikeastaan tarvitse tätä kurssia varten." onko näin?
* Tuo esille, että tekoälyä saa käyttää muuten kuin ratkaisujen tuottamiseen

## Materiaali

* Enemmän kuvallisia esimerkkejä siitä miten verkkoalgoritmit toimivat
* Verkkoalgoritmien toteutukset ilman `float("inf")`-trikkiä, voisi toimia niin että ääretöntä etäisyyttä ei ole tallennettu
* Tuo esille, miten lyhimpiä polkuja etsitään suuntaamattomassa verkossa (nyt esimerkeissä vain suunnattuja)
* Tuo esille, että verkossa voi olla useita samanlaisia kaaria sekä kaari solmusta itseensä
* Pythonissa `set` ei säilytä alkioita suuruusjärjestyksessä vaikka voi näyttää siltä, esimerkki tästä materiaaliin
* Maininta `heapq.heapify`-funktiosta. Tällöin esim. tehtävä ["Pienimmät alkiot"](https://cses.fi/tira24k/task/2539) voisi korostaa paremmin heapsortin ideaa
* Historiallisia (?) aiheita: linkitetty lista, pikajärjestäminen, binäärihaku, binäärihakupuu
* Esittele materiaalissa hyvin: `enumerate`, `zip`, `defaultdict`, listakooste, `for _ in`, `pprint` (?), mieti muutenkin
* Tuo paremmin esille, mitä $O$-merkintä tarkoittaa ja että sitä voi käyttää muutenkin kuin aikavaativuuksissa
* Miten laskea tarkasti suurilla kokonaisluvuilla (esim. `/` on epätarkka mutta `//` on tarkka)
* Bittioperaatiot ja binäärijärjestelmän hyödyntäminen algoritmeissa
* Ford-Fulkersonin tehokkuuteen liittyvä esimerkki on epäselvä, koska materiaalin toteutus ei toimi esimerkin mukaisesti.

## Tehtävät

* Tuo esille kaikissa tehtävissä selkeästi, kuinka tehokas algoritmin tulisi olla (esim. “algoritmin tulee toimia tehokkaasti kun ruudukon koko on 100”)
* Voisiko testi kartoittaa ratkaisun suoritusaikaa, ja verrata sitä odotettuun? Tavoitteena hyödyllisempi palaute kuin "oli liian hidas". Esim. sovittamalla syötearvo→aika eri asteisiin polynomeihin, ja tutkimalla millä näistä korrelaatio oli paras. Ideaalinen palaute: "It looks like your function count has the running time complexity O(n²). Its running time complexity should be O(n log n) or better."
* Avoimissa tehtävissä monet vastaukset ovat huonoja/vääriä, pitäisi parantaa vastausten tarkastusta tai luopua näistä tehtävistä
* Avoimissa tehtävissä on myös opiskelijoille epäselvää, milloin voi menettää pisteen tehtävästä
* Olisiko tarvetta tietorakenteiden simulointiin?
* Paranna tiedotusta siitä, että joka viikko tulee ratkaista vähintään x tehtävää
* Binäärihakupuutehtävät mahdollista saada testeistä läpi koodilla jossa ei ole binääripuuta -> muuta testejä niin ettei tämä ole mahdollista (miten?)
* Tehtävä “Kaikki puut” (3103): monella googletettu (?) kaava jota ei ymmärretä
* Tehtävä “Robotti“ (3441): epäselvää mistä kyse tehtävässä, kuvitus ja/tai lyhempi testisyöte voisi auttaa
* Tehtävä “Laskut“ (3458): tietyt ratkaisut eivät mene läpi PyPyllä mutta menevät läpi CPythonilla
* Tehtävä “Esiintymismäärät“ (3483): pääsee läpi koodilla, joka käy läpi `count`-kutsussa kaikki eri esiintymismäärät
* Tehtävä “Läpikäynti“ (3544): pääsee läpi koodilla, joka käyttää set-rakennetta (12744528) 
* Tehtävä “Seinät ja lattiat“ (3561): pääsee läpi hitaalla koodilla
* Jos testattavalla funktiolla tai luokalla on sivuvaikutuksia, joiden johdosta se toimii oikein ensimmäisellä kutsulla mutta ei muiden testien jälkeen, tämä tulisi näyttää selvästi
  - Miten tämän voisi tarkastaa luotettavasti?
* Jos funktion parametri on lista tms. tietorakenne, tulisi varmistaa, että funktio ei muuta tietorakennetta
  - Tämä tarkastus tulisi tehdä kaikkiin tehtäviin
* Tuo esille, että käytettävissä on Pythonin standardikirjasto mutta ei esim Numpy
* Tuo esille CPythonin ja PyPyn versiot ja näiden erot
* Erottele aikarajan ylityksessä yksittäisen testin aikarajan ylitys ja kokonaisuuden aikarajan ylitys
* Muuta tehtäväpohjia niin ettei ole syntaksivirheitä (esim. `pass`-komennot)
* Ylimääräinen viikko tehtäviä, joissa ei kerrota mihin aiheeseen liittyy?
* Kurssilla ei tulisi olla kahta tehtävää, joilla on samanniminen kooditiedosto

## Palautetta II-osasta keväältä 2024

* Luku 9, teoria: Olisi hyvä selittää, mitä '' tarkoittaa tässä yhteydessä: return count_sequences(n - 1, d + 1) +
count_sequences(n - 1, d - 1)
* Luku 11, teoria: Pitäisikö "Liukuva ikkuna" esimerkissä lukea selityksessä "Lisäksi jos havaitaan, että keon pienin alkio on jäänyt listan ulkopuolelle, se poistetaan keosta", niin sanan 'listan' sijasta 'osalistan' (eli se ikkuna)?
* Tehtävä 10-8 "Kurssi": Pitäisikö tehtävän annossa mainita, että kaikki kurssit ovat saatavilla/tehtävissä välittömästi? Eli ei samaan tapaan kuten Tira-kurssilla 2x8 kerrallaan ja viikon päästä seuraavat 2x8.
* Tehtävä 11-8 "Pienet summat": Tehtävänantoa pitää selventää huomattavasti, esim. pitäisi laittaa suoraan esimerkkinä vastaukset n arvoilla 1-5. Discordissakin vastaukset vinkkeihin sarjan alusta vaihtelevat, niin on vaikea päätellä mikä on oikea alku.
* Tehtävä 12-2 "Puun korkeus": Jos tehtävänannossa funktio on muotoa "def height(self):" ja mallivastauksessa "def height(self, node=None):", niin se on aika hämäävää ja herkästi laittaa yrittämään tehtäviä siten, että funktion parametriosasto ei muutu koska tulee tunne ettei se mene testeistä läpi jos sitä muuttaa.
* Tehtävä 12-4 "Edellinen ja seuraava": Tässä pitäisi selventää, että viitataan "suurin pienempi" ja "pienin suurempi" konsepteihin.
* Tehtävä 12-7 "Monta alkiota": Pitäisi selventää, että myös luokkaa Node saa muuttaa! Nyt teksti on: "Muuta kurssimateriaalin luokkaa TreeSet niin, että sama alkio voi toistua monta kertaa. Tämä vaatii muutoksia materiaalin metodeihin." Mainitaan kyllä, että metodeihin pitää koskea, mutta ei muihin luokkiin. Tästä saa vaikutelman, että testit feilaavat jos Node-luokkaan koskee, koska annetussa koodi-rungossa ei myöskään näy Node-luokkaa. Lisäksi, mallivastauksen metodit "add" ja "contains" on toteutettu rekursiolla kun materiaalissa while-loopissa, mikä sotkee ajatuksia kun kerrotaan että "idea on vain muuttaa" Node-luokkaa ja kaikki metodit näyttävätkin eriltä kuin materiaalissa.
* Tehtävä 14-8 "Veden mittaus": Pitäisikö mainita, että a, b ja c ovat kokonaislukuja?
* Luku 16, teoria: "Edmonds-Karp" -algoritmin yhteydessä O(nm) ei ole mainittu mikä "n" on, oletan että solmujen määrä?
* Luku 16, teoria: "Maksimiparitus", selityksessä voisi mainita että tarkoitus on löytää maksimimäärä solmupareja. Tämä tulee kyllä ilmi tanssiaiset-esimerkistä, mutta sitä edeltävä selitys "Verkon maksimiparitus (maximum matching) on suurin mahdollinen kaarten joukko, jossa pätee, että jokainen solmu kuuluu enintään yhteen kaareen" on melko abstrakti.

