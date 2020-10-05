=======================================
Language of Data hand-annotated corpora
=======================================

These hand-annotated corpora contain two special kinds of text extracted from structured (CSV-based) Open Data datasets:
 - headers: CSV column header text;
 - data: CSV textual data attributes.

Data sources:
 - data.gov.uk (English)
 - data.illinois.gov (English)
 - data.gov.au (English)
 - dati.trentino.it (Italian)
 - dati.comune.milano.it (Italian)

For details on the data collection, curation, and annotation process, please see our paper:
Gábor Bella, Linda Gremes, and Fausto Giunchiglia. Exploring the Language of Data. Proceedings of COLING 2020. https://www.researchgate.net/publication/344451391_Exploring_the_Language_of_Data

The tab-separated TSV files use the following format in each separate line:
original_string <TAB> annotated_string

The following annotations are provided:
 - tokenisation;
 - part-of-speech tags separated from the words by a space (using the Penn POS tags for English and the ISST-TALN tagset for Italian);
 - instead of "proper noun" tags, the following named entity tags are provided, using BI notation (joint POS-NER tagging):
    - PER: persons,
    - ORG: organisations,
    - GPE: geopolitical entities and locations,
    - DAT: dates and times,
    - ADD: postal addresses,
    - WWW: web addresses,
    - EML: email addresses,
    - MSC: miscellaneous.

Please cite our paper if you reuse this work in any way.
Please respect the licensing terms included in the bundle.
