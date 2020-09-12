# The Pile™

The Pile is (going to be) the world's largest open source language modeling data set. We are currently developing Version 1, with a goal of 1 TiB of English text.

|    Component    |   Size   |Weight|Epochs|Mean Document Size|
|-----------------|----------|------|-----:|------------------|
|Bibliotik        |100.96 GiB|29.59%| 3.276|538.36 KiB        |
|ArXiv            |56.21 GiB |16.48%| 3.276|46.61 KiB         |
|FreeLaw          |51.15 GiB |14.99%| 3.276|57.08 KiB         |
|OpenWebText      |37.03 GiB |10.85%| 3.276|4.84 KiB          |
|PubMed Abstracts |19.26 GiB |5.65% | 3.276|1.30 KiB          |
|Wikipedia (en)   |17.27 GiB |5.06% | 3.276|3.00 KiB          |
|OpenSubtitles    |12.98 GiB |3.81% | 3.276|30.48 KiB         |
|Gutenberg (PG-19)|10.88 GiB |3.19% | 3.276|398.73 KiB        |
|Literotica       |8.81 GiB  |2.58% | 3.276|24.39 KiB         |
|DM Mathematics   |7.75 GiB  |2.27% | 3.276|47.21 MiB         |
|BookCorpus       |6.30 GiB  |1.85% | 3.276|369.87 KiB        |
|Ubuntu IRC       |5.52 GiB  |1.62% | 3.276|15.96 MiB         |
|CORD-19          |4.26 GiB  |1.25% | 3.276|25.59 KiB         |
|NIH ExPorter     |1.89 GiB  |0.56% | 3.276|2.11 KiB          |
|Enron Emails     |901.43 MiB|0.26% | 3.276|1.78 KiB          |
|**Total**        |341.15 GiB|      |      |10.38 KiB         |


(Epochs refers to the number of epochs elapsed after 1.2TB)



## Manual Download Components

The following components need manual downloading. Either download them or comment out from `pile.py`. 

 - **Bibliotik**: `books3.tar.gz` needs to be in the current directory. Download temporarily unavailable.
 - **CORD-19**: `document_parses` needs to be in the current directory. Download from [here](https://www.kaggle.com/allen-institute-for-ai/CORD-19-research-challenge).

## Workflow

To propose a new dataset be added to the Pile, [open an issue](https://github.com/EleutherAI/The-Pile/issues/new). Your issue should include a description of the dataset, its size, what language(s) it is in, a link to the data, and any other relevant information. If a project manger approves your proposal, they will change its label to [![Datasets](https://img.shields.io/github/labels/EleutherAI/The-Pile/Dataset)](https://github.com/EleutherAI/The-Pile/labels/Dataset) and add it to [![Project: Datasets](https://img.shields.io/badge/Project-Datasets-lightgrey)](https://github.com/EleutherAI/The-Pile/projects/2). Datasets that we elect to not include in the current version of the Pile will receive a [![Deferred](https://img.shields.io/github/labels/EleutherAI/The-Pile/Deferred%20to%20v2)](https://github.com/EleutherAI/The-Pile/labels/Deferred%20to%20v2) or [![Declined](https://img.shields.io/github/labels/EleutherAI/The-Pile/Declined)](https://github.com/EleutherAI/The-Pile/labels/Declined) label. While we welcome multilingual  datasets and plan on including non-English datasets in the future, the initial release of the Pile will be English-only and all submissions of non-English datasets will be deferred.

To claim responsibility for implementing an unclaimed dataset, leave a comment on one of our unassigned issues. Once an dataset has been assigned to you, make the necessary changes to `datsets.py` and `pile.py` in a fork and submit a pull request. If you require, you can also submit a script for processing the data as shown [here](https://github.com/EleutherAI/pile_enron_emails).

To raise an issue that is not proposing a new dataset, open an issue with the tag [![Feature Request](https://img.shields.io/github/labels/EleutherAI/The-Pile/Feature%20Request)](https://github.com/EleutherAI/The-Pile/labels/Feature%20Request) or [![Bug](https://img.shields.io/github/labels/EleutherAI/The-Pile/Bug)](https://github.com/EleutherAI/The-Pile/labels/Bug) as appropriate.
