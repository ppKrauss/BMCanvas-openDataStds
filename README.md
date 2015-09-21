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

This proposal use the Open Knowledge's [Data Packaged Core Datasets](https://github.com/datasets) conventions (as well [W3C conventions for CSV](http://www.w3.org/TR/tabular-data-model/)) for store data in a [five-star open format](http://5stardata.info/en/), preserving its full-access. Among Datasets conventions the file [datapackage.json](datapackage.json) offer all metadata of CSV files.

## Popular models and standard models
There are many BMCanvas variants, and in this project is not possible to describe all of them here. Therea are some *curatory process* to select the "most popular" or "most representative" canvas variations.  Any discussion must start with a Canvas metadata descriptors, at [refModels.csv](./data/refModels.csv), and consensual [evidence](./data/evidence) &mdash; a image illustration preserved in this repo as an evidence to the structure and terminology used in the reference model &mdash; to build the ofther descriptions. 

## Terminology and semantics

The concepts list is at [def-elements.csv](./data/def-elements.csv). The terms used to express each concept is language-dependent, so, is defined only at specific canvas definition (see "Canvas main description" below), and without a central normalization. Only the *element labels* are the commom for all specifications.

## Canvas main description
All files with prefix `def` are definitions.  The suffix is the canvas label (defined in  [refModels](./data/refModels.csv)), them a [IETF language label](https://github.com/datasets/language-codes/blob/master/data/ietf-language-tags.csv). Examples:
* [def-std2009-ptBR.csv](./data/def-std2010-ptBR.csv), a Brazilian Portuguese (ptBR) Standard Canvas descrition.
* [def-std2009-en.csv](./data/def-std2009-en.csv), a English (en) Standard Canvas descrition.
* [def-lean2010-ptBR.csv](./data/def-lean2010-ptBR.csv),  a ptBR Lean Canvas descrition.
* ...

### Structure representation
The proposal is restricted to the usual design solutions, and the "usual" theme variations. So, as pointed by Wikipedia and others, the reference model is the [Strategyzer.com canvas](https://commons.wikimedia.org/wiki/File:Business_Model_Canvas.png), that is a table with 9 cells. Any other "variant canvas structure" of this project must by expressed as a "table os cells".

The most simple and human-readable way to express formally the structure (to after use as "machine recipe" in template or design transcriptors) is to express the canvas in a CSV file and indicate the cells that must be merged, by a "left span" or "above span" commands in the merged cells. All the cells can be supposed in a balanced distribution, without lost of semantics &mdash; the simetry or widthes can be free for each application.

So, to read and undertand the structure specification you only need to remember that the arrow symbols ("↑", "←", etc.) are prefixes for reserved words, as "↑span" and "←span". Example: compare the  [`std2009` structure specification](./data/strut-std2009.csv) with [its evidence](./data/evidence/std2009.png).

For each `def` file there are a generic (language independent) structure. Examples:
* [strut-std2009.csv](./data/strut-std2009.csv) is reference for [def-std2009-ptBR.csv](./data/def-std2010-ptBR.csv) and [def-std2009-en.csv](./data/def-std2009-en.csv);
* [strut-lean2010.csv](./data/strut-lean2010.csv) for  [def-lean2010-ptBR.csv](./data/def-lean2010-ptBR.csv), ...

