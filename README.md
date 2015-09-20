# BMCanvas-openDataStds
Business Model Canvas, a proposal of simple Open Data Standards


## Objectives and motivations
[Business Model Canvas](https://en.wikipedia.org/wiki/Business_Model_Canvas), or **BMCanvas**, is a well-accepted and popular language to express Business Models... As any other language, it is subject to the effects of the [Tower of Babel](https://en.wikipedia.org/wiki/Tower_of_Babel). There are many tutorials (ex. more tham 3000 tutorials at youtube) and many APPs (more tham 100 sites that offer specialized canvas editors), etc.

In each one of this BMCanvas content or application, it is possible to detect some kind of "variant" of terminology, structure, concept or methodology. Users and developers have a lack of reference models and recommendations about this variants. This project is a proposal to fill this lack. However, the focus here is limited to the project objectives:

* promote a *standard terminology* into the BMCanvas variants;
* offer a *referential* (and labels) about main variants and semantics;
* describe the *canvas structure* of each variant;
* offer *support for data-interchange* (import/export, etc.) of BMCanvas of different APPs or enviroments.

# The conventions
Below, the standard. The formal specifications are distrubuted into (friendly) CSV and JSON files, all in a collaborative `git` context.

This proposal use the Open Knowledge's [Data Packaged Core Datasets](https://github.com/datasets) conventions (as well [W3C conventions for CSV](http://www.w3.org/TR/tabular-data-model/)) for store data in a [five-star open format](http://5stardata.info/en/), preserving its full-access.


## Popular models and standard models
... intro ... Any discussion must refer a consensual [evidence](./data/evidence).

File [refModels.csv](./data/refModels.csv) show the reference models and fix its labels, to distinguisg different Canvas strutures (or arrangement of concepts) and use in the other filenames. In this CSV the column `local_img` is a image illustration preserved in this repo as an evidence to the structure and terminology used in the reference model.

## Coventions about terminology and semantics

The concept list is not normalized, but expressed one set of concepts for each refModel-language. Anyway, the *element labels* are the commom for all descriptions, so, as in Wikipedia, we can expect a "concept consensus" between languages (in the *element* definition). All files with prefix "BMCanvasDef" are definitions.  Examples:

* [def-std2009-ptBR.csv](./data/def-lean2010-ptBR.csv), a Brazilian Portuguese Standard Canvas descrition.
* [def-lean2010-ptBR.csv](./data/def-lean2010-ptBR.csv),  a Brazilian Portuguese Lean Canvas descrition.
* ...

## Canvas structure representation
The proposal is restricted to the usual design solutions, and the "usual" theme variations. So, as pointed by Wikipedia and others, the reference model is the [Strategyzer.com canvas](https://commons.wikimedia.org/wiki/File:Business_Model_Canvas.png), that is a table with 9 cells. Any other "variant canvas structure" of this project must by expressed as a "table os cells".

The most simple and human-readable way to express formally the structure (to after use as "machine recipe" in template or design transcriptors) is to express the canvas in a CSV file and indicate the cells that must be merged, by a "left span" or "above span" commands in the merged cells. All the cells can be supposed in a balanced distribution, without lost of semantics &mdash; the simetry or widthes can be free for each application.

So, to read and undertand the structure specification you only need to remember that the arrow symbols ("↑", "←", etc.) are prefixes for reserved words, as "↑span" and "←span". Example: compare the  [`std2009` structure specification](./data/strut-std2009.csv) with [its evidence](./data/evidence/std2009.png).

