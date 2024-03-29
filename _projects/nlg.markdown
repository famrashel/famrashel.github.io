---
layout: project
title: nlg package
description: A Python library for analogy purpose.
---

A Python library for analogy purpose.
- Vector representation of words
- Extraction of analogical clusters from a set of words
- Construction of analogical grids
- Analogical equation solver

The main purpose of this library is to construct analogical grids from a given set of strings.

#### Word forms → analogical grids
Each word form is represented as a vector with
the number of occurrences of all the characters in the alphabet.

<!-- ![Word forms to analogical grids]({{site.url}}/img/projects/word_to_grid.png) -->

<img src="{{ site.baseurl }}/img/projects/word_to_grid.png" alt="word_forms_to_nlggrids">
<span class="caption text-muted">
	Using the number of occurrences of charaters as the formal level of vector representation
</span>

#### Morphological features → paradigm tables
By using morphological features as the vector representation,
the output is paradigm tables.

<img src="{{ site.baseurl }}/img/projects/morph_to_paratab.png" alt="morphology_to_paradigm">
<span class="caption text-muted">
	Using the morphological features, e. g. POS tag, of the word form as vector representation
</span>

#### User-defined features → new type of grids
It is possible to use your own features.
For example, we can combine:
- the number of occurrences of all the characters
- morphological features

<img src="{{ site.baseurl }}/img/projects/form+morph.png" alt="form_morph_to_regular">
<span class="caption text-muted">
	Using both the formal and morphological levels as vector representation to organise regular conjugations
</span>

#### Future work: word embeddings → semantical analogical grids
The limitation of this library is that the value of the vector representation is integer.
The future work of this library is to be able to accept floating numbers.
Thus,
we can use word embeddings to construct semantical analogical grids.

<img style="text-align: center;" src="{{ site.baseurl }}/img/projects/semantic_grid.png" alt="embeddings_to_semantic_grid">
<span class="caption text-muted">
	Using word embeddings as input to construct semantical analogical grids
</span>

### Code
GitHub repository: <https://github.com/famrashel/nlg.git>

There is a Jupyter notebook which illustrates some basic usages of the package mentioned above.

### Publication
Rashel Fam and Yves Lepage.
**Tools for the production of analogical grids and a resource of n-gram analogical grids in 11 languages**.
In Proceedings of the *11th edition of the Language Resources and Evaluation Conference (LREC 2018)*, pages 1060–1066, Miyazaki, Japan, May 2018.
[Download](https://aclanthology.org/L18-1171)