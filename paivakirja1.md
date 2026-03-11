# Oppimispäiväkirja: Paikallinen git

__Mikä osion tehtävissä oli vaikeaa ja mikä helppoa? Mikä auttoi minua oppimaan? Miten selvitin esteet?__

Olin jo tuttu Gitin peruskomentojen kanssa ja hallitsen ne hyvin. Uuden oppimisessa auttoi käytännön harjoittelu, sen avulla komennot ja niiden toiminta jäivät hyvin mieleen. Helpoin oli esimerkiksi komento git log, jolla voi nähdä historian, mikä on erittäin kätevää. Haasteena oli se, että täytyy työskennellä huolellisesti, jotta välttyy virheiltä tai sekaannuksilta, mutta on olemassa myös komentoja kuten restore ja revert. Vaikka se ei ollut vaikeaa, oli silti tärkeää ymmärtää ero staged- ja committed-tilojen välillä.

## Osiossa käyttämäni Git-komennot

| Komento                         | Kuvaus                |
| --------------------------------| ----------------------|
|git init                         |luo uuden Git-repositorion nykyiseen kansioon|
|git clone url                    |kopioi olemassa olevan ulkoisen arkiston tietokoneelle uuteen kansioon|
|git status                       |näyttää repositorion nykyisen tilan|
|git add tiedosto                 |lisää tietyn tiedoston staging-kohtaan|
|git add .                        |lisää kaikki uudet ja muutetut tiedot staging-kohtaan|
|git commit                       |luo commitin siitä, mikä on jo lisätty stagingiin|
|git commit -m 'kommentti'        |tekee commitin heti komentorivillä olevan viestin tekstin kanssa|
|git log                          |näyttää commit-historiat|
|git log --stat                   |näyttää commit-historian ja lyhyen yhteenvedon|
|git diff tiedosto                |näyttää nykyisen tiedostoversion ja viimeksi tallennetun version välisen eron                         
|git rm tiedosto                  |poistaa tiedoston sekä työkansiosta että Git-arkistosta|
|git mv vanha_nimi uusi_nimi      |nimeää tiedoston uudelleen|
|git tag nimi                     |luo tagin nykyiselle commitille|
|git checkout hash                |vaihtaa repositorion tilan määritetyn commitin tilaan sen hash-arvon perusteella|
|git switch -                     |palauttaa takaisin edelliseen haaraan tällaisen vaihdon jälkeen|
|git switch -c new-branch-name    |luo uuden haaran ja siirtyy siihen|
|git reset tiedosto               |poistaa tiedoston staging-kohdasta|
|git reset                        |poistaa stagingista kaikki sinne lisätyt muutokset|
|git reset --hard                 |hylkää kaikki tallentamattomat muutokset työkansiossa|
|git restore tiedosto             |peruuttaa tallentamattomat muutokset tietyssä tiedostossa ja palauttaa sen viimeisimpään tallennettuun versioon|
|git revert hash                  |luo uuden commitin, joka kumoa määritetyn commitin muutokset|
|git log -2                       |näyttää vain kaksi viimeisintä commitia|
|mkdir kansio                     |luo uuden kansion|
|cd kansio                        |siirtyy määritettyyn kansioon|
|ls -a                            |näyttää tiedostot, myös piilotetut|
|ls -l                            |näyttää yksityiskohtaisen luettelon tiedostoista|
|la -l -a                         |näyttää yksityiskohtaisen luettelon tiedostoista, myös piilotetuista|
|rm tietosto                      |tiedoston poistaminen|
|mv lähde kohde                   |tiedoston siirtäminen|
