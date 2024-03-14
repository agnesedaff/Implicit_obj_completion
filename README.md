This repository contains the complete annotated corpus, results and scripts used for my master thesis' project on the authomatic completion of Implicit Arguments in Italian at the University of Pavia (academic year 2022/2023).

TITLE:
"Authomatic Implicit Object Completion in Italian: an exploration with BERT".

ABSTRACT:
This thesis describes an experiment on automatic Implicit Object completion in Italian. The
task is structured as a _fill-mask_ or _cloze-task_ to be applied to five Italian BERT models, fully
exploiting their bidirectional capabilities. Firstly, starting from a selected Ontology of 30
verbs (37 semantic patterns from the T-PAS resource), a corpus of 1.200 sentences is created.
The corpus is divided into two datasets, called EXPLICIT and IMPLICIT. The second dataset,
containing Implicit Objects, is manually annotated by two experts with both a _Gold Standard_
(GS) Noun and the type of omission occurring, understood as a _Defaulting_ strategy that can
apply either lexically or pragmatically (Jezek, 2018). The manual annotation shows a
significant correlation between the type of _Defaulting_ and the range of possible completions
for each verb. Subsequently, the experiment is applied and the results are evaluated by
calculating the cosine similarity between the model's output and the manual GS completion. It
is demonstrated that the model _bert-base-italian-xxl-cased_ performs better than lighter models
in the task, thanks to its ability to guess the most frequent collocations in _Lexical Defaulting_
contexts. It is confirmed what has been observed in previous studies, namely that BERT
models tend to favor the frequency of _n-grams_, with some difficulty in completing the Object
when a deeper understanding of semantic relationships is required (e.g., output = "Il postino
suona \[il pianoforte\] sempre due volte"). Furthermore, it is observed that the models tend to
return words in metonymic relation to the GS, replicating the mechanism of _semantic
coercion_ (Pustejovsky and Jezek, 2008), and possess limited sensitivity to linguistic
boundaries in the explicitation of _Shadow Arguments_.

The corpus has also been presented at the conference CliC-it 2023 with the paper:

Daffara, Agnese e Jezek, Elisabetta (2023). Towards an Italian Corpus for Implicit Object Completion. In _Proceedings of the ninth Italian Conference on Computational Linguistics CliC-it 2023_, Venice, Italy. https://ceur-ws.org/Vol-3596/paper19.pdf 

