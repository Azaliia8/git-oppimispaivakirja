# Oppimispäiväkirja: Paikallinen git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet?__

Olin jo tuttu Gitin peruskomentojen kanssa ja hallitsen ne hyvin. Uuden oppimisessa auttoi käytännön harjoittelu, sen avulla komennot ja niiden toiminta jäivät hyvin mieleen. Helpoin oli esimerkiksi komento git log, jolla voi nähdä historian, mikä on erittäin kätevää. Haasteena oli se, että täytyy työskennellä huolellisesti, jotta välttyy virheiltä tai sekaannuksilta, mutta on olemassa myös komentoja kuten restore ja revert. Vaikka se ei ollut vaikeaa, oli silti tärkeää ymmärtää ero staged- ja committed-tilojen välillä.

## Osiossa käyttämäni Git-komennot

| Komento                         | Kuvaus                |
|---------------------------------|-----------------------|
|mkdir demo                       |luo uuden hakemiston|
|cd demo                          |siirtyy hakemistoon demo|
|git tag harjoitus2               |lisää viimeisimpään commitiin tunnisteen harjoitus2|
|git init                         |luo uuden Git-repositorion nykyiseen hakemistoon|
|git clone url                    |kloonaa olemassa olevan repositorion omalle koneelle|
|git status                       |näyttää repositorion nykyisen tilan|
|git add tiedosto                 |lisää tiedoston seuraavaan talletukseen|
|git add .                        |lisää kaikki nykyisen hakemiston uudet ja muuttuneet tiedostot seuraavaan talletukseen|
|git commit                       |tekee talletuksen ja avaa editorin commit-viestin kirjoittamista varten|
|git commit -m "kommentti"        |tekee talletuksen ja lisää kommenttiviestin suoraan komentoriviltä|
|git log                          |näyttää commit-historian|
|git log --stat                   |näyttää commit-historian ja lisäksi yhteenvedon siitä, mitä tiedostoja kommiteissa muuttui|
|git diff tiedosto                |näyttää tiedoston muutokset verrattuna viimeksi talletettuun versioon|
|git mv vanha_nimi uusi_nimi      |nimeää tiedoston uudelleen|
|git mv uusinimi.txt newdir       |siirtää tiedoston uusinimi.txt hakemistoon newdir.|
|git tag nimi                     |luo tagin nykyiselle commitille|
|git checkout hash                |vaihtaa repositorion tilan määritetyn commitin tilaan sen hash-arvon perusteella|
|git switch -                     |palauttaa takaisin edelliseen haaraan tällaisen vaihdon jälkeen|
|git switch -c new-branch-name    |luo uuden haaran ja siirtyy siihen|
|git reset tiedosto               |poistaa tiedoston staging-alueelta|
|git reset                        |Poistaa staging-alueelta kaikki sinne lisätyt muutokset|
|git reset --hard                 |hylkää kaikki tallentamattomat muutokset työkansiossa|
|git restore tiedosto             |peruuttaa tallentamattomat muutokset tietyssä tiedostossa ja palauttaa sen viimeisimpään tallennettuun versioon|
|git revert hash                  |luo uuden commitin, joka kumoaa määritetyn commitin muutokset|
|git log -2                       |näyttää vain kaksi viimeisintä commitia|
|mkdir kansio                     |luo uuden kansion|
|ls -a                            |näyttää tiedostot, myös piilotetut|
|ls -l                            |näyttää yksityiskohtaisen luettelon tiedostoista|
|ls -l -a                         |näyttää kaikki tiedostot, myös piilotetut, sekä tarkemmat tiedot niistä|
|git rm tiedosto                  |poistaa tiedoston sekä työhakemistosta että Git-hallinnasta|
|mv lähde kohde                   |siirtää tiedoston paikasta toiseen tai nimeää sen uudelleen|
|git branch testing               |luo uuden haaran nimeltä testing|
|git branch                       |näyttää olemassa olevat paikalliset haarat|
|git log --graph --all --oneline  |näyttää commit-historian graafisena ja tiiviinä näkymänä kaikista haaroista|
|git switch master                |siirtyy master-haaraan|
|git merge iss53                  |yhdistää haaran iss53 muutokset nykyiseen haaraan|
|git merge --abort                |keskeyttää keskeneräisen yhdistämisen konfliktitilanteessa|
