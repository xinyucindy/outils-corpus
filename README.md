# Outils de traitement de corpus — Master Plurital

## Pratique

6 séances les lundis de 9h à 12h dans l'amphi 5 de l'INALCO, PLC, 65 rue des grands moulins, 75013 Paris.

## Évaluation

Un devoir à rendre après chaque séance. La note finale sera la moyenne des notes.

## Séances

### 18 mars 2019
* [intro, définitions](outils_corpus-1.pdf)
* [formats d'annotations, outils de requêtes](outils_corpus-2.html)


[Kafka_metamorphosis](files/kafka-metamorphosis_gutenberg.txt)

[Kafka_metamorphosis treetagger](files/kafka-metamorphosis_gutenberg_treetagger.txt)

#### devoir : trouver 3 corpus et les définir avec les 6 critères vus en cours


### 25 mars 2019
* [types, tokens, mots](outils_corpus-3.html)
* [extraction d'informations](outils_corpus-4.html)

#### devoir : calculer le ratio type/token pour les discours sur l'état de l'Union de [2016](files/stateoftheunion2016.txt) et [2017](files/stateoftheunion2017.txt)

Pour la tokenization, utilisez le [tokenizer de Stanford](https://nlp.stanford.edu/software/tokenizer.shtml), [NLTK](http://www.nltk.org) ou [Spacy](https://spacy.io/)
Vous devez envoyer le résultat ainsi que la description de vos traitements (scripts, outils, …)

### 1er avril 2019

* [graphes, grew, spacy](outils_corpus-5.html)
  * [Graphs in Python](https://www.python-course.eu/graphs_python.php)
  * [Python Patterns - Implementing Graphs](https://www.python.org/doc/essays/graphs/)

#### devoir : À l'aide de spacy extrayez les triplets (sujet, verbe, objet) des phrases suivantes et commentez les éventuelles erreurs ou manques.
 - « Le chat mange la souris. »
 - « Les enfants n'aiment pas trop les asperges. »
 - « Les Français réclament moins d'impôts. »
 - « Les acacias donnent un miel ambré, limpide et fluide. »
 - « L'équipe fait porter le chapeau à l'arbitrage. »


### 8 avril 2019

* [spacy](outils_corpus-6.html)

#### devoir : au choix
 - Modifiez le script de vectorisation du cours d'[introduction à la fouille textes](https://loicgrobol.github.io/intro-fouille-textes/) de façon à (1) utiliser la tokenisation par Spacy et (2) ajouter un trait comptant le nombre d'entités nommées par documents.
 - Ré-entraînez un modèle pour l'adapter à : soit deux textes de chansons en français « non standard » (hip-hop, français de la francophonie, …), soit deux poésies de François Villon ([exemple](https://www.poetica.fr/poeme-5050/francois-villon-ballade-des-dames-du-temps-jadis/)) ou de textes de la même époque.
 Étiquetez soit en POS, soit en EN.

### 15 avril 2019

* [étiquetage](outils_corpus-7.html)

#### devoir : Étiquetez manuellement puis avec l'étiqueteur de votre choix les deux textes suivants. Calculez la précision globale pour chacun des textes et commentez.
[sequoia.txt](files/sequoia.txt), [bashung.txt](files/bashung.txt)

Vous pourrez utiliser le [script d'évaluation de CoNLL 2018](http://universaldependencies.org/conll18/evaluation.html) (attention aux formats d'entrée), ce [script](https://github.com/dtuggener/ComparEval/blob/master/pos_tagging/eval_pos_tagger.py) ou vos propres calculs.


### 6 mai 2019

* [word embeddings](outils_corpus-8.html)
* liens
  * [exemples de génération de texte avec OpenAi](https://openai.com/blog/better-language-models/)
  * [génération de fanfiction Harry Potter](https://twitter.com/JanelleCShane/status/1097652984316481537)
  * [exemple amusant sur Pride and Prejudice](http://www.ghostweather.com/files/word2vecpride/)

## Références

  * Tony McEnery and Andrew Wilson. Corpus  Linguistics. Edinburgh: Edinburgh University Press, 2001 (second edition).
  * Céline Poudat et Frédéric Landragin. Explorer un corpus textuel : Méthodes – pratiques – outils. De Boeck Supérieur, 2017.
  * Daniel Jurafsky and James H. Martin.Speech and Language Processing. Pearson, 2008 (second edition). [pdfs de la troisième édition en cours](https://web.stanford.edu/~jurafsky/slp3/)
  * [Lecture Slides from the Stanford Coursera course by Dan Jurafsky and Christopher Manning](https://web.stanford.edu/~jurafsky/NLPCourseraSlides.html)
  * [Site de Sébastien Ruder](http://ruder.io/)
  * [Cours interactif sur Spacy par Ines Montani](https://course.spacy.io/)