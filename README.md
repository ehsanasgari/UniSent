# UniSent: Universal Adaptable Sentiment Lexica for 1000+ Languages

We introduce UniSent universal sentiment lexica for 1000+ languages. Sentiment lexica are vital for sentiment analysis in absence of document-level annotations, a very common scenario for low-resource languages. To the best of our knowledge, UniSent is the
largest sentiment resource to date in terms of
the number of covered languages, including many
low resource ones. In this work, we use a massively parallel Bible corpus to project sentiment information from English to other languages for sentiment analysis on  Twitter data.
We introduce a method called DomDrift to mitigate the huge domain mismatch between Bible and Twitter by a confidence weighting scheme that uses domain-specific embeddings to compare the nearest neighbors for a candidate sentiment word in the source (Bible) and target (Twitter) domain.
We evaluate the quality of UniSent in a subset of languages for which manually created ground truth was available, Macedonian, Czech, German, Spanish, and French. We show that the quality of UniSent is comparable to manually created sentiment resources when it is used as the sentiment seed for the task of word sentiment prediction on top of embedding representations. In addition, we show that emoticon sentiments could be reliably predicted in the Twitter domain using only UniSent and monolingual embeddings in German, Spanish, French, and Italian. With the publication of this
paper, we release the UniSent sentiment lexica.


If you use the resource please cite the arxiv version of the UniSent paper (submitted to the LREC 2020):
```
@article{asgari2019unisent,
  title={UniSent: Universal Adaptable Sentiment Lexica for 1000+ Languages},
  author={Asgari, Ehsaneddin and Braune, Fabienne and Ringlstetter, Christoph and Mofrad, Mohammad RK},
  journal={arXiv preprint arXiv:1904.09678},
  year={2019}
}
```

# The provided resources

## 1. UniSent lexcia is available at 'unisent_lexica_v1' 
Along with the paper, we release the UniSent sentiment lexica for 1242 unique languages. The lexicon files are located at "unisent_lexica_v1/xxx_unisent_lexicon.txt", where the "xxx" is the language ISO 639-3 codes. The mapping between the ISO code and the language name can be found in unisent_languages.xlsx. 


## 2.  unisent_languages.xlsx
A complete list of 1242 unique languages covered by UniSent along with their language family information is provided in the supplementary material.



## The corpus of 1000 languages  

The super-parallel corpus of 1000+ can be found here:

https://github.com/ehsanasgari/1000Langs

```
@inproceedings{asgari-schutze-2017-past,
    title = "Past, Present, Future: A Computational Investigation of the Typology of Tense in 1000 Languages",
    author = {Asgari, Ehsaneddin  and
      Sch{\"u}tze, Hinrich},
    booktitle = "Proceedings of the 2017 Conference on Empirical Methods in Natural Language Processing",
    month = sep,
    year = "2017",
    address = "Copenhagen, Denmark",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/D17-1011",
    doi = "10.18653/v1/D17-1011",
    pages = "113--124",}

```