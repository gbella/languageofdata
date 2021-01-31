
We succinctly call the **Language of Data** the unique grammar of short textual labels that typically appear in structured data. For example:

<sub>Name</sub> | <sub>Full_addr</sub> | <sub>Type</sub> | <sub>Notes</sub>
----------------|----------------------|-----------------|-----------------
<sub>Pizza Rio</sub> | <sub>Via della Resistenza, 9/A, 38123 Trento, Italy</sub> | <sub>pizzeria</sub> | <sub>take-away possible</sub>
<sub>La Bigoudène</sub> | <sub>18 rue Vauban, 29200 Brest, France</sub> | <sub>pancake restaurant</sub> | <sub>Closed Permanently</sub>

Both headers and data values in the dataset above have the following characteristics:

* **short labels**, consisting of just a few words;
* **frequent named entities** (names, postal addresses, dates, URLs);
* **non-standard orthography** (use of "\_" for token separation, Inconsistent Use of Capitals, frequent abbreviations, etc.);
* **absence or rarity of certain parts of speech** (e.g. verbs, pronouns);
* **non-standard syntax** (omission of verbs, prepositions, inverted word order, etc.: _take-away \[is\] possible_, _operate \[an\] uninsured vehicle_, _death country_.

## Why is this special grammar relevant?

A high-accuracy automated analysis of the textual content of vast datasets is crucial in many applications, such as information retrieval (e.g. for meaning-based indexing of content by search engines), data integration, or AI-based data analytics.

## Why is it so hard to parse the Language of Data?

State-of-the-art natural language processing tools are trained on regular text (e.g. Wikipedia) or on social media content (e.g. tweets). They analyse text _in context_, looking at a window of preceding and following words and phrases. In the Language of Data, context is short or non-existent, and orthography and syntax are used in specific, non-standard ways. Conventional NLP tools vastly underperform on such text (e.g. 10-40% of F-measure for named entity recognition, 70% of accuracy in classifying parts of speech). The specific grammar of the Language of Data needs specifically designed NLP tools.

## Resources and tools

Our corpora and tools are in their early stages and are under constant development. More resources will follow in the near future.
All tools and corpora are licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/), meaning that you are free to share and adapt the material for non-commercial purposes, provided that you give appropriate credit to the authors. Do not hesitate to [contact us](mailto:thelanguageofdata@gmail.com) for individual licensing arrangements. 

### Trained NLP models

Name | Version | Task | Language | Accuracy/F1 | Link
-----|---------|------|----------|-------------|-----
LoD OpenNLP Tokenizer  | 1.0 | tokenization | English | 96.7% | [Download](https://github.com/gbella/languageofdata/tree/main/download/en_tokenizer_lod.bin)
LoD OpenNLP POS Tagger | 1.0 | POS tagging  | English | 85.9% | [Download](https://github.com/gbella/languageofdata/tree/main/download/en_postagger_lod.bin)
LoD OpenNLP Name Finder| 1.0 | NER          | English | 50.8% | [Download](https://github.com/gbella/languageofdata/tree/main/download/en_ner_lod.bin)
LoD BERT-NER           | 1.0 | NER          | English | 67.4% | coming soon

Note that sequence labelling classification tasks such as POS or NER tagging are much harder over the Language of Data, which explains the difference w.r.t. state-of-the-art scores over regular text.

### Corpora

Name | Description | Language | Nb. labels | Nb. tokens | Link
-----|-------------|----------|------------|------------|-----
LoD Headers English | Hand-annotated table head labels extracted from English-language Open Data catalogues. Token boundaries, POS and NER tags. | English | 8,558 | 31,127 | [Download](https://github.com/gbella/languageofdata/tree/main/download/lod_eng_headers_annotated_0.9.zip)
LoD Data English | Hand-annotated data value labels extracted from English-language Open Data catalogues. Token boundaries, POS and NER tags. | English | 8,731 | 39,698 | [Download](https://github.com/gbella/languageofdata/tree/main/download/lod_eng_data_annotated_0.9.zip)
LoD Headers Italian | Hand-annotated table head labels extracted from Italian-language Open Data catalogues. Token boundaries, POS and NER tags. | Italian | 3,536 | 9,723 | [Download](https://github.com/gbella/languageofdata/tree/main/download/lod_ita_headers_annotated_0.9.zip)
LoD Data Italian | Hand-annotated data value labels extracted from Italian-language Open Data catalogues. Token boundaries, POS and NER tags. | Italian | 6,528 | 39,517 | [Download](https://github.com/gbella/languageofdata/tree/main/download/lod_ita_data_annotated_0.9.zip)


## Publications

<div style="background-color: #f0f0c0; padding: 7pt;">
<p style="font-weight: bold">The main publication supporting our principal hypotheses, please cite this if you use our resources or tools.</p>
<p>
<a href="https://www.researchgate.net/publication/344451391_Exploring_the_Language_of_Data" target="_blank">Gábor Bella, Linda Gremes, and Fausto Giunchiglia. <span style="font-weight: bold">Exploring the Language of Data.</span> Proceedings of COLING 2020.</a>
</p>
</div>

An early publication on using NLP mechanisms tailored to the Language of Data in order to perform multilingual and multi-domain word sense disambiguation:

[Gábor Bella, Alessio Zamboni, and Fausto Giunchiglia. _Domain-Based Sense Disambiguation on Multilingual Structured Data._ Proceedings of the ECAI 2016 workshop on Diversity Aware Artificial Intelligence, The Hague, Netherlands.](http://www.ecai2016.org/content/uploads/2016/08/W13-diversity-2016.pdf#page=59)


## Credits

Research on the Language of Data is being carried out at the [Language Diversity Lab](http://knowdive.disi.unitn.it/language-diversity/) of the [KnowDive Research Group](http://knowdive.disi.unitn.it) at the [University of Trento](http://www.unitn.it), Italy. For any inquiry, do not hesitate to [drop us an email](mailto:thelanguageofdata@gmail.com).

Contributors:

* [Gábor Bella](http://sites.google.com/site/gaborbellaphd);
* prof. [Fausto Giunchiglia](http://disi.unitn.it/~fausto);
* Linda Gremes.
