---
annotations_creators:
- crowdsourced
language:
- en
language_creators:
- found
license:
- cc-by-nc-sa-3.0
multilinguality:
- monolingual
pretty_name: Answer Sentence Natural Questions (ASNQ)
size_categories:
- 10M<n<100M
source_datasets:
- extended|natural_questions
task_categories:
- multiple-choice
task_ids:
- multiple-choice-qa
paperswithcode_id: asnq
---

# Dataset Card for "asnq"

## Table of Contents
- [Dataset Description](#dataset-description)
  - [Dataset Summary](#dataset-summary)
  - [Supported Tasks and Leaderboards](#supported-tasks-and-leaderboards)
  - [Languages](#languages)
- [Dataset Structure](#dataset-structure)
  - [Data Instances](#data-instances)
  - [Data Fields](#data-fields)
  - [Data Splits](#data-splits)
- [Dataset Creation](#dataset-creation)
  - [Curation Rationale](#curation-rationale)
  - [Source Data](#source-data)
  - [Annotations](#annotations)
  - [Personal and Sensitive Information](#personal-and-sensitive-information)
- [Considerations for Using the Data](#considerations-for-using-the-data)
  - [Social Impact of Dataset](#social-impact-of-dataset)
  - [Discussion of Biases](#discussion-of-biases)
  - [Other Known Limitations](#other-known-limitations)
- [Additional Information](#additional-information)
  - [Dataset Curators](#dataset-curators)
  - [Licensing Information](#licensing-information)
  - [Citation Information](#citation-information)
  - [Contributions](#contributions)

## Dataset Description

- **Homepage:** [https://github.com/alexa/wqa_tanda#answer-sentence-natural-questions-asnq](https://github.com/alexa/wqa_tanda#answer-sentence-natural-questions-asnq)
- **Repository:** [More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
- **Paper:** [TANDA: Transfer and Adapt Pre-Trained Transformer Models for Answer Sentence Selection](https://arxiv.org/abs/1911.04118)
- **Point of Contact:** [More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
- **Size of downloaded dataset files:** 3398.76 MB
- **Size of the generated dataset:** 3647.70 MB
- **Total amount of disk used:** 7046.46 MB

### Dataset Summary

ASNQ is a dataset for answer sentence selection derived from
Google's Natural Questions (NQ) dataset (Kwiatkowski et al. 2019).

Each example contains a question, candidate sentence, label indicating whether or not
the sentence answers the question, and two additional features --
sentence_in_long_answer and short_answer_in_sentence indicating whether ot not the
candidate sentence is contained in the long_answer and if the short_answer is in the candidate sentence.

For more details please see
https://arxiv.org/abs/1911.04118

and

https://research.google/pubs/pub47761/

### Supported Tasks and Leaderboards

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Languages

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

## Dataset Structure

### Data Instances

#### default

- **Size of downloaded dataset files:** 3398.76 MB
- **Size of the generated dataset:** 3647.70 MB
- **Total amount of disk used:** 7046.46 MB

An example of 'validation' looks as follows.
```
{
    "label": 0,
    "question": "when did somewhere over the rainbow come out",
    "sentence": "In films and TV shows ( edit ) In the film Third Finger , Left Hand ( 1940 ) with Myrna Loy , Melvyn Douglas , and Raymond Walburn , the tune played throughout the film in short sequences .",
    "sentence_in_long_answer": false,
    "short_answer_in_sentence": false
}
```

### Data Fields

The data fields are the same among all splits.

#### default
- `question`: a `string` feature.
- `sentence`: a `string` feature.
- `label`: a classification label, with possible values including `neg` (0), `pos` (1).
- `sentence_in_long_answer`: a `bool` feature.
- `short_answer_in_sentence`: a `bool` feature.

### Data Splits

| name  | train  |validation|
|-------|-------:|---------:|
|default|20377568|    930062|

## Dataset Creation

### Curation Rationale

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Source Data

#### Initial Data Collection and Normalization

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

#### Who are the source language producers?

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Annotations

#### Annotation process

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

#### Who are the annotators?

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Personal and Sensitive Information

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

## Considerations for Using the Data

### Social Impact of Dataset

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Discussion of Biases

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Other Known Limitations

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

## Additional Information

### Dataset Curators

[More Information Needed](https://github.com/huggingface/datasets/blob/master/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)

### Licensing Information

The data is made available under the Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License:
https://github.com/alexa/wqa_tanda/blob/master/LICENSE

### Citation Information

```
@article{Garg_2020,
   title={TANDA: Transfer and Adapt Pre-Trained Transformer Models for Answer Sentence Selection},
   volume={34},
   ISSN={2159-5399},
   url={http://dx.doi.org/10.1609/AAAI.V34I05.6282},
   DOI={10.1609/aaai.v34i05.6282},
   number={05},
   journal={Proceedings of the AAAI Conference on Artificial Intelligence},
   publisher={Association for the Advancement of Artificial Intelligence (AAAI)},
   author={Garg, Siddhant and Vu, Thuy and Moschitti, Alessandro},
   year={2020},
   month={Apr},
   pages={7780–7788}
}
```

### Contributions

Thanks to [@mkserge](https://github.com/mkserge) for adding this dataset.
