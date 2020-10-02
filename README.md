
## What is the Language of Data?

We succinctly call _the Language of Data_ the unique grammar of short textual labels that typically appear in structured data. For example:

Name | Full_addr | Type | Notes
-----|-----------|------|------
Pizza Rio | Via della Resistenza, 9/A, 38123 Trento, Italy | pizzeria | take-away possible
La Bigoudène | 18 rue Vauban, 29200 Brest, France | pancake restaurant | Closed Permanently

Both headers and data values in the dataset above have the following characteristics:

* labels are short, consisting of just a few words;
* named entities (proper nouns) are frequent;
* orthography is non-standard (use of "\_" for token separation, Inconsistent Use of Capitals, frequent abbreviations, etc.);
* some categories of words are rarely or almost never used (e.g. verbs, pronouns);
* syntax is often non-standard (omission of verbs, prepositions, etc.: _take-away \[is\] possible_).

## Why is this special grammar relevant?

The automated analysis of the text content of vast datasets is crucial in many applications, such as information retrieval (e.g. for meaning-based indexing of content by search engines), data integration, or AI-based data analytics.

## Why is it so hard to parse the Language of Data?

State-of-the-art natural language processing tools are trained on standard language consisting of full sentences, e.g. Wikipedia. They analyse text _in context_, looking at a window of preceding and following words and phrases. In the Language of Data, context is short or non-existent, and orthography and syntax are non-standard. Conventional NLP tools vastly underperform on such text (e.g. 10-40% of F-measure for named entity recognition, 70% of accuracy in classifying parts of speech). The specific grammar of the Language of Data needs specifically designed NLP tools.

## Resources and tools for parsing the Language of Data

TODO

## Publications

The main publication supporting our principal hypotheses, please cite this if you use our resources or tools.

[Gábor Bella, Linda Gremes, and Fausto Giunchiglia. _Exploring the Language of Data._ Proceedings of COLING 2020.](https://www.researchgate.net/publication/344451391_Exploring_the_Language_of_Data)

An early publication on using NLP mechanisms tailored to the Language of Data in order to perform multilingual and multi-domain word sense disambiguation:

[Gábor Bella, Alessio Zamboni, and Fausto Giunchiglia. _Domain-Based Sense Disambiguation on Multilingual Structured Data._ Proceedings of the ECAI 2016 workshop on Diversity Aware Artificial Intelligence, The Hague, Netherlands.](http://www.ecai2016.org/content/uploads/2016/08/W13-diversity-2016.pdf#page=59)


## Credits

TODO

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
