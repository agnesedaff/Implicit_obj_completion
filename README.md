This repository contains the complete annotated corpus, results and scripts used for my master thesis' project at the University of Pavia (academic year 2022/2023).

TITLE

Ita: "Completamento automatico dell’Oggetto Implicito in italiano: un’esplorazione con BERT"

Eng: "Authomatic Implicit Object Completion in Italian: an exploration with BERT".

ABSTRACT

Ita: La tesi descrive un esperimento sul completamento automatico dell’Oggetto Implicito in
italiano. Il task è strutturato come un _fill-mask_ o _cloze-task_ da applicare a cinque modelli
BERT italiani, sfruttando appieno le loro capacità bidirezionali. In primis, a partire da
un’Ontologia scelta di 30 verbi (37 pattern semantici della risorsa T-PAS), viene creato un
corpus di 1.200 frasi. Il corpus è diviso in due dataset, chiamati EXPLICIT e IMPLICIT. Il
secondo dataset, contenente Oggetti Impliciti, viene annotato manualmente da due esperti con
un sostantivo _Gold Standard_ (GS) e il tipo di omissione, intesa come una strategia di
_Defaulting_ che può avvenire a livello lessicale o pragmatico (Jezek, 2018). Dall’annotazione
manuale emerge una correlazione significativa tra il tipo di _Defaulting_ e il range di possibili
completamenti per ogni verbo. Successivamente, tale risorsa viene utilizzata per applicare
l’esperimento e i risultati sono valutati calcolando la _cosine similarity_ tra l’output dei modelli
e il completamento manuale GS. Si dimostra che il modello _bert-base-italian-xxl-cased_
funziona meglio dei modelli più leggeri nel task, grazie alla capacità di indovinare le
collocazioni più frequenti nei contesti di _Defaulting_ lessicale. Viene confermato quanto
osservato in studi precedenti, ovvero che i modelli BERT tendono a privilegiare la frequenza
degli _n-grams_, con alcune difficoltà a completare l’Oggetto laddove è necessaria una
comprensione più profonda delle relazioni semantiche (es. output = “Il postino suona \[il
pianoforte\] sempre due volte”). Si osserva inoltre la tendenza dei modelli a restituire parole in
relazione metonimica con il GS, replicando il meccanismo di _semantic coercion_ (Pustejovsky
e Jezek, 2008), e la scarsa sensibilità ai limiti linguistici nell’esplicitazione degli _Shadow
Arguments_.

Eng: This thesis describes an experiment on automatic Implicit Object completion in Italian. The
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

It also contains the material for our paper presented at CliC-it 2023:

Daffara, Agnese e Jezek, Elisabetta (2023). Towards an Italian Corpus for Implicit Object Completion. In _Proceedings of the ninth Italian Conference on Computational Linguistics CliC-it 2023_, Venice, Italy. https://ceur-ws.org/Vol-3596/paper19.pdf 

