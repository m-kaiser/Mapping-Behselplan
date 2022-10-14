# Mapping the Behselplan (1822–1825)

Starting point was the georeferencing of address numbers, the so called “Konskriptionsnummern” (conscription numbers, valid during 1770 and 1860), depicted on the city map of the city building inspector and cartographer [Anton Behsel (1781–1838)]( https://www.geschichtewiki.wien.gv.at/index.php?title=Anton_Behsel&oldid=827981). Behsel worked between 1822 and 1825 on his map which includes not only the city of Vienna but also the surrounding suburbs. This could be done on the basis of the georeferenced map tiles provided by the [map services of the city of Vienna](https://www.data.gv.at/katalog/dataset/7462373e-aac4-4582-9b2f-ad760b568ed4). The points were placed in [QGIS]( https://www.qgis.org/de/site/) on the original spot of the plan numbers. It resulted in 7,380 map points.

Each of the point data were then collated with the addresses mentioned in the address book published at the same time by Anton Behsel. Due to the rapid city growth, the addresses shifted several times. Behsel organised his concordance around three time slices: 
- newest (1822–1860)
- older (1795–1821)
- oldest (1770–1794)

By linking them to the address book, it was possible to transfer Behsel’s address concordance. Finally, this dataset not only provides georeferenced addresses for a specific time period. It will also be possible to use the dataset for the identification and localization of earlier addresses, which could be found in historical source materials.

![image of network node](https://github.com/m-kaiser/Mapping-Behselplan/blob/main/Mapping_Behsel_Preview.png)
> Screenshot showing the mapping of the Behselplan (background layer with building polygons from the [Franziszeischen Kataster](https://www.data.gv.at/katalog/dataset/4030d796-0573-4305-86f2-b34e38a86a1d))

## Dataset

| column title | definition |
|--------------|------------|
| id | unique identifier for the table |
| Adresse | joined values from column G (Gassen und Plätze/streets and squares) and column C (Hausnummern/addresses)|
| Hausnummer | address number (newest according to Behsel) |
| alte_1795_1821 | concordance with older address numbers |
| ältere_1770_1795 | concordance with oldest address numbers |
| Hausinhaber | column from Behsel's address book, seldom transcribed, only if an institution is mentioned |
| Gassen und Plätze | historical names for street and squares |
| Grundobrigkeit | public authority responsible for the land register |
| Latitude | geocoordinates for latitude, 7 decimal places 7 digest long  |
| Longitude | geocoordinates for longitude, 7 decimal places 7 digest long |
| Planinhalt | city aeras shown in a specific map tile |
| Vorstadt_Stadviertel | suburb or district |
| reference | abbreviated citation of the source map|
| WienWiki_Pagetitle | original title of the page in Vienna History Wiki |
| WienWiki_Permalink | permalink to the entry in Vienna History Wiki |

## Sources

Anton Behsel, Stadtplan von Wien und seinen Vorstädten (1820-1825), [WStLA, Pläne und Karten: Sammelbestand, P1: 295G](https://www.wien.gv.at/actaproweb2/benutzung/archive.xhtml?id=Stueck++00001994ma8KartoSlg#Stueck__00001994ma8KartoSlg). 
Anton Behsel, Verzeichniß aller in der kaiserl. königl. Haupt- und Residenzstadt Wien mit ihren Vorstädten befindlichen Häuser, Wien: Gedruckt und im Verlage Bey Carl Gerold, 1829. [urn:nbn:at:AT-WBR-7003](https://resolver.obvsg.at/urn:nbn:at:AT-WBR-7003).
