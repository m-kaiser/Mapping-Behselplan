# Mapping the Behselplan (1822–1825)

Starting point was the georeferencing of address numbers, the so called “Konskriptionsnummern” (conscription numbers, valid during 1770 and 1860), depicted on the city map of the cartographer [Anton Behsel (1781–1838)]( https://www.geschichtewiki.wien.gv.at/index.php?title=Anton_Behsel&oldid=827981). Behsel worked between 1822 and 1825 on his map which includes not only the city of Vienna but also the surrounding suburbs. This could be done on the basis of the georeferenced map tiles provided by the [map services of the city of Vienna](https://www.data.gv.at/katalog/dataset/7462373e-aac4-4582-9b2f-ad760b568ed4). The points were placed in [QGIS]( https://www.qgis.org/de/site/) on the original spot of the plan numbers. It resulted in 7,380 map points.

Each of the point data were then collated with the addresses mentioned in the address book published at the same time by Anton Behsel. Due to the rapid city growth, the addresses shifted several times. Behsel organised his concordance around three time slices: 
- newest (1822–1860)
- older (1795–1821)
- oldest (1770–1794)

By linking them to the address book, it was possible to transfer Behsel’s address concordance. Finally, this dataset not only provides georeferenced addresses for a specific time period. It will also be possible to use the dataset for the identification and localization of earlier addresses, which could be found in historical source materials.

![image of network node](https://github.com/m-kaiser/Mapping-Behselplan/blob/main/Mapping_Behsel_Preview.png)
> Screenshot showing the mapping of the Behselplan (background layer with building polygons from the [Franziszeischen Kataster](https://www.data.gv.at/katalog/dataset/4030d796-0573-4305-86f2-b34e38a86a1d))

## Decription
- points (mapping of the map tiles)
- addresses (transcription of the concordance)
- dataset (linked dataset consisting of points and adresses)

### Points

| column title | definition |
|--------------|------------|
| id | unique identifier for the table |
| Adresse | joined values from column G (Gassen und Plätze/streets and squares) and column C (Hausnummern/adresses)|
| Hausnummer | adress number (newest according to Behsel) |
| alte_1795_1821 | concordance with older adress numbers |
| ältere_1770_1795 | concordance with oldest adress numbers |
| Hausinhaber | column from Behsel's adress book, seldom transcribed, only if an institution is mentioned |
| Gassen und Plätze | historical names for street and squares |
| Grundobrigkeit | public authority responsible for the land register |
| Latitude | Breitengrad |
| Longitude | Längengrad |
| Vorstadt | suburb |
| reference | abbreviated citation of the source map|








