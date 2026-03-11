# Oppimispäiväkirja: Hajautettu git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet, jotka vaikuttivat tehtävän suorittamiseen?__

Helpointa oli ladata projekti omalle paikalliselle repositoriolle, lähettää omat muutokset, hakea päivitykset ja tarkistaa, mihin yhteys oikein menee. Nämä asiat olivat hyvin loogisia ja jo ennestään tuttuja. Toisessa osiossa helpointa oli ymmärtää GitHub, GitLab ja Bitbucket, joita käytetään repositorioiden säilyttämiseen internetissä ja projektien yhteiseen kehittämiseen. Myös README-tiedoston idea projektin etusivuna oli melko helppo ymmärtää.

Uutta oli oppia ero fetch- ja pull-komentojen välillä: fetch vain hakee muutokset, kun taas pull yhdistää ne heti nykyiseen haaraan. Uutta oli myös ymmärtää, että origin/master on etähaaran paikallisesti tallennettu esitys fetch-komennon jälkeen. Myös origin + upstream -malli voi aluksi hämmentää: mistä muutokset haetaan, minne ne viedään ja miksi upstream-haaraan ei voi tehdä push-komentoa. Uutta olivat myös käsitteet self hosting ja cloud hosting.

Oppimista auttoivat komentojen lyhyet esimerkit ja tietenkin käytännön harjoittelu uuden materiaalin kanssa. Termien selitykset auttoivat oppimisessa.

Varsinaisia ongelmia ei tullut vastaan, mutta mahdollisia konflikteja voisi syntyä pull-komennon yhteydessä, jos paikalliset ja etämuutokset menevät päällekkäin. Oli tärkeää olla sekoittamatta Git:iä ja GitHubia.

## Osiossa käyttämäni Git-komennot

| Komento                            | Kuvaus |
| -----------------------------------| ------------------------------|
|git remote add origin url           |Lisää etärepositorion nimellä origin|
|git remote                          |Näyttää etärepositorioiden nimet.|
|git remote -v                       |Näyttää etärepositorioiden nimet ja niiden osoitteet.|
|git remote rename origin temp       |Nimeää etärepositorion origin uudelleen nimelle temp.|
|git remote rm temp                  |Poistaa etärepositorion nimeltä temp.|
|git remote show origin              |Näyttää yksittäisen etärepositorion tiedot. |
|git fetch                           |Hakee muutokset etärepositoriosta ilman automaattista yhdistämistä.|
|git fetch origin                    |Näyttää etähaarat.|
|git checkout master                 |Siirtyy master-haaraan.|
|git merge                           |Yhdistää muutokset nykyiseen haaraan.|
|git merge origin/master             |Yhdistää etähaaran origin/master muutokset nykyiseen paikalliseen haaraan.|
|git pull origin                     |Hakee muutokset etärepositoriosta ja yhdistää ne heti.|
|git push                            |Vie nykyisen haaran etärepositorioon.|
|git push origin master              |Vie paikallisen master-haaran etärepositorioon.|
|git push -—all                      |Vie kaikki paikalliset haarat etärepositorioon.|
|git push -u origin master           |Vie master-haaran ja asettaa sille yhteyden etähaaraan.|
|git push -u origin feat123          |Vie uuden feat123-haaran etärepositorioon ja asettaa sille upstream-yhteyden.|
|git push --delete origin feat123`   |Poistaa haaran etärepositoriosta.|
|git branch --delete feat123`        |Poistaa paikallisen haaran.|
|git log                             |Näyttää commit-historian.|