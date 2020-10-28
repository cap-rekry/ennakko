# Rekry-ennakkotehtävä

### Luo versionhallintaan oma kehityshaara ja toteuta seuraava tehtävä:

0. Esivalmistelut
	
	0.1 Ota käyttöön migrations-kansion default.sql:n sisältämät tietokannan taulut

	0.2 Resetoi rekry@cap.fi-käyttäjän salasana ja kirjaudu sisään wp-adminiin

1. Asenna Custom Post Type UI -plugin
	
	1.1 Luo custom post_type: Kirjat / book

2. Asenna Advanced Custom Fields -plugin

	2.1 luo book-post_typelle kaksi lisäkenttää:
		* Arvosana (1-5)
		* Tila: lainassa, hyllyssä, hukassa (pakollinen tieto)

3. Luo sivu, jonka osoite on /kirjahylly/ ja joka toimii book-post_typen arkistosivuna
	
	3.1. Lisää tietokantaan muutamia esimerkkikirjoja sekä anna niille arvosana ja määritä tila.

	3.2. Tulosta arkistosivulla allekkain kaikki kirjat niin, että kirjasta näkyy Kirjan nimi (the_title), arvosana ja tila.

	3.3. Muokkaa arkisto-sivun Main Query:a niin, että sivulla tulostetaan vain kirjat, joille on määritetty arvosana

	3.4. Lisää sivun alkuun filtteri-kenttä, johon voi kirjoittaa tekstiä. Filtteröi kirjoja reaaliaikaisesti vertaamalla kirjan nimeä ja filtteri-kenttään syötettyä tekstiä (filtteri "taru" näyttää siis mm. kirjat "Taru sormusten herrasta" ja "Eldoradon taru")

4. Tee pull request muutoksista
	
	4.1. Lisää pull requestin mukana (migrations-kansioon) mahdolliset migraatio-ohjeet ja tietokannan dumppi


### Huomioitavaa:

Tee muutokset niin, että ne eivät katoa, kun Twenty Twenty -teema päivitetään.

Kirjan single-näkymästä ei tarvitse huolehtia tässä tehtävässä.