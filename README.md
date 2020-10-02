
## What is the Language of Data?

We succinctly call _the Language of Data_ the unique grammar of short textual labels that typically appear in structured data. For example:

Name | Full_addr | Type | Notes
-----|-----------|------|------
Pizza Rio | Via della Resistenza, 9/A, 38123 Trento, Italy | pizzeria | take-away possible
La Bigoudène | 18 rue Vauban, 29200 Brest, France | pancake restaurant | Closed Permanently

Both headers and data values in the dataset above have the following characteristics:

* **short labels**, consisting of just a few words;
* **frequent named entities** (names, postal addresses, dates, URLs);
* **non-standard orthography** (use of "\_" for token separation, Inconsistent Use of Capitals, frequent abbreviations, etc.);
* **absence or rarity of certain parts of speech** (e.g. verbs, pronouns);
* **non-standard syntax** (omission of verbs, prepositions, inverted word order, etc.: _take-away \[is\] possible_, _operate \[an\] uninsured vehicle_, _death country_.

## Why is this special grammar relevant?

A high-accuracy automated analysis of the textual content of vast datasets is crucial in many applications, such as information retrieval (e.g. for meaning-based indexing of content by search engines), data integration, or AI-based data analytics.

## Why is it so hard to parse the Language of Data?

State-of-the-art natural language processing tools are trained on standard language (e.g. Wikipedia) or on social media content (e.g. tweets). They analyse text _in context_, looking at a window of preceding and following words and phrases. In the Language of Data, context is short or non-existent, and orthography and syntax are used in specific, non-standard ways. Conventional NLP tools vastly underperform on such text (e.g. 10-40% of F-measure for named entity recognition, 70% of accuracy in classifying parts of speech). The specific grammar of the Language of Data needs specifically designed NLP tools.

## Resources and tools

Our corpora and tools are in their early stages and are under constant development. More resources will follow in the near future.

### Trained NLP models

Name | Version | Task | Language | Accuracy/F1 | Link
-----|---------|------|----------|-------------|-----
OpenNLP Tokenizer  | 1.0 | tokenization | English | 96.7% | TODO
OpenNLP POS Tagger | 1.0 | POS tagging  | English | 85.9% | TODO
OpenNLP Name Finder| 1.0 | NER          | English | 50.8% | TODO
BERT-NER           | 1.0 | NER          | English | 67.4% | TODO

### Corpora

Name | Description | Language | Nb. labels | Nb. tokens | Link
-----|-------------|----------|------------|------------|-----
LoD Open Data English | Hand-annotated labels extracted from English-language Open Data catalogues. Token boundaries, POS and NER tags. | English | 17,289 | 70,825 | TODO
LoD Open Data Italian | Hand-annotated labels extracted from Italian-language Open Data catalogues. Token boundaries, POS and NER tags. | Italian | 14,277 | 49,240 | TODO

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

Research on the Language of Data is being carried out at the [Language Diversity Lab](http://knowdive.disi.unitn.it/language-diversity/) of the [KnowDive Research Group](http://knowdive.disi.unitn.it) at the [University of Trento](http://www.unitn.it), Italy.

Contributors:

* [Gábor Bella](http://sites.google.com/site/gaborbellaphd) (lead);
* prof. [Fausto Giunchiglia](http://disi.unitn.it/~fausto);
* Linda Gremes.

<!--
You can use the [editor on GitHub](https://github.com/gbella/languageofdata/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/gbella/languageofdata/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
-->
