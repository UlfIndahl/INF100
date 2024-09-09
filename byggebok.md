# INF100 - Jupyterbook Guide


## Pushe filer til Github

* Gjøre: Save all (i filmenyen)
* Lage en commit i Github Dekstop med endringene som er gjort med en beskrivende tittel
* "Commit to master"
* Push to Origin
* Kan sjekke at OK via "master" i min Github.
* Da skal endringene som er gjort være tilgjengelig på Github, men boka er ikke oppdatert

## Bygge bok og publisere bok til Github Pages

* Kjøre kommando (muligens to ganger): jupyter-book clean --all .
* Kjøre kommandoen for å bygge boka: jupyter-book build --all . 
    * Hvis du ønsker å se på nettsiden før du publiserer til Github så kan du gå inn i _build/html/index.html i nettleseren
* For å publisere til Github Pages: ghp-import -n -p -f ./_build/html 

I tilfelle du trenger mer informasjon om hvordan å publisere boka på Github Pages:  https://jupyterbook.org/en/stable/start/publish.html 