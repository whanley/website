---
title: "Datasets to share"
date: 2019-02-15
description: "This is meta description of datasets"
type: "featured"
image: "images/featured-post/garlic.jpg"
categories:
  - "Datasets"
tags:
  - "github"
  - "indexes"
---

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br />This <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" rel="dct:type">work</span> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

I'm committed to data sharing and reuse. The data listed below is the product of transformations I've done myself, using various tools: OpenRefine, especially, but also regex editing in batches.

I've tried to post descriptions, changelogs, and data dictionaries in the github repositories. I'm getting better at doing this work systematically, but it's a hard habit to establish. I'm also trying to post releases via Zenodo, so that each data repository has a [DOI](https://en.wikipedia.org/wiki/Digital_object_identifier).

The material is in a variety of formats: mostly plain text (`csv`, `tsv`), some XML, some Turtle (`.ttl`) for RDF use, and some OpenRefine projects.

*Quantity* and *Quality* are shorthand fields meant to offer a quick sense of each dataset. Quantity is number of records or, in the case of tabular datsets, rows x columns. Quality is graded A-D, and refers to the amount of ordering, checking, cleaning, parsing, and enrichment that I've achieved. In other words, it's a measure of my confidence that the data I present represents the content of the original analogue sources.

### Person Names (Egypt)
doi: [10.5281/zenodo.4628298](https://doi.org/10.5281/zenodo.4628298)
Name | Year(s) | Format(s) | Quantity | Quality | Link | Source   
---|---|---|---|---|---|---
British Subjects in Alexandria | 1888    | csv, ttl      | 1084 x 16 | A  | [github directory](https://github.com/whanley/names-data/tree/master/british-subjects-alexandria-1888) | National Archives of the United Kingdom, FO 881/5968                      
Indicateur Egyptien | 1897    | csv           | 6200 x 25 | A  | [github directory](https://github.com/whanley/names-data/tree/master/indicateur-egyptien-1897)         | [Poffandi, Stefano G., ed. *1897 Indicateur Égyptien Administratif et Commercial*. 11th ed. (Alexandria: Imprimerie Générale, 1896)](https://gallica.bnf.fr/ark:/12148/bpt6k58024532)
Tunisians in Egypt   | 1881-4  | csv, tsv, ttl | 303 x 52 | A | [github directory](https://github.com/whanley/names-data/tree/master/tunisians-egypt-1881)             | Filib Jallad, Qamus al-idarah wa-al-qadaʾ, 3rd ed. (Cairo: Matbaʿat Dar al-Kutub wa-al-Wathaʾiq al-Qawmiyah, 2003), 2:296–300;  Ministère des Affaires Étrangères, Centre des Archives Diplomatiques de Nantes - Fonds Alexandrie: Recensement—Tunisiens 69/69–73. |

### Ottoman Placenames
doi: [10.5281/zenodo.4660215](https://doi.org/10.5281/zenodo.4660215)
Name | Year(s) | Format(s) | Quantity | Quality | Link | Source   
---|---|---|---|---|---|---
Ottoman administrative divisions|13th-20th centuries| tsv, ttl | 11989 x 25 | A | [tsv](https://github.com/whanley/Ottoman-Gazetteer/tree/master/data/archived-versions), [ttl](https://github.com/whanley/Ottoman-Gazetteer/blob/master/data/ottgaz.ttl), [data dictionary](https://github.com/whanley/Ottoman-Gazetteer/blob/master/data/metadata_dictionary.md) | Tahir Sezen's [Osmanlı Yer Adları](http://www.os-ar.com/osmanli_yer_isimleri.pdf)
Ottoman place names | 1530 | tsv | 121080 x 13 | C | [github directory](https://github.com/whanley/Ottoman-Gazetteer/tree/master/data/1530-places) | to be supplied
Ontology | 13th - 20th centuries | ttl | 7 | C | [github directory](https://github.com/whanley/Ottoman-Gazetteer/tree/master/ontology) | me

### Egypt historical data
doi: [10.5281/zenodo.4660261](https://doi.org/10.5281/zenodo.4660261)
Name | Year(s) | Format(s) | Quantity | Quality | Link | Source   
---|---|---|---|---|---|---
Census tables, Alexandria|1897, 1907, 1917|csv| |B|[github directory](https://github.com/whanley/egypt-data/tree/main/alexandria-census)|originals

to come:
- Alexandria export data|1905
- Italian indemnities|1882|
- Tribunaux mixtes personnel|

### International Law Journals
doi: [10.5281/zenodo.4660225](https://doi.org/10.5281/zenodo.4660225)
Name | Year(s) | Format(s) | Quantity | Quality | Link | Source   
---|---|---|---|---|---|---
Bulletin de la Société de législation comparée|1869-1939|TEI-XML|404 issues|C|[github directory](https://github.com/whanley/ilcorpus/tree/master/journals/bslc)|various facsimiles
Journal du droit international privé et de la jurisprudence comparée (Clunet)|1874-1939|TEI-XML|324 issues|C|[github directory](https://github.com/whanley/ilcorpus/tree/master/journals/clunet)|various facsimiles
Revue de droit international et de législation comparée|1869-1939|TEI-XML|65 volumes|C-|[github directory](https://github.com/whanley/ilcorpus/tree/master/journals/rdilc)|various facsimiles
