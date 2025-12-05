---
layout: default
title: Portfolio
---

# DocuLens

DocuLens on lähetyslistojen digitalisointiohjelmisto, jonka avulla skannatut lähetyslistat voidaan ladata sovellukseen, niiden sisältävää tietoa voi tarkastella, muokata ja tallentaa. Esimiesnäkymässä (admin) pystyy myös näkemään ja tarkastelemaan valmiita, jo tarkastettuja lähetyslistoja.

# Alku
Projektin alussa Angular osaamista ei ollut ja ymmärrys hyvästä projektin kansiorakenteesta ja modulaarisuudesta olivat vähäisiä. API interaktioista oli vain pientä tietoa ja GitHub osaaminen oli olematonta.

# Oma kontribuutio
Oma roolini oli frontend kehittäjä, joten olin vastuussa frontend puolen toiminnallisuudesta. Testaajan rooli siirtyi itseltä pois kesken projektin työmäärän jaon tasauksen seurauksena.

# Mitä opin

## Tiimityöskentely
Jotain tänne

## Projektin hallinta
Jotain tänne

## Uudet oivallukset
Vanhan korjaus / parannus kun enemmän osaamista löytyy

### Esimerkkinä storen käytön välttely

Koska sovelluksen data perustuu API kutsuihin (joka sivulla päivitetty data haetaan tietokannasta), ei sovelluksella ollut mitään jaettavaa dataa komponenttien välillä. Tähän ainoina poikkeuksina oli id:n siirto yhdeltä sivulta toiselle ja admin näkymä, joka simuloi eri käyttäjien näkymiä eri sivuilla (Admin näkee enemmän tietoa).\n

Ratkaisuna molemmissa tapauksissa käytin reittiparametreja, koska ajattelin tapauksien olevan niin pienimuotoisia, että ne ei tarvitsisi erillistä storea (josta en Angularissa tiennyt mitään). Tämä laiskuus myöhemmässä vaiheessa kostautui itselle, kun admin näkymä laajeni kaikille sivuille, jolloin jouduin reitityksen ja reittiparametrien kanssa tappelemaan, jotka ei lopulta jokaisessa tilanteessa toiminut. Jos tälle olisin alunperin tehnyt storen, niin tuleva ominaisuuden laajentaminen olisi ollut paljon yksinkertaisempaa.
