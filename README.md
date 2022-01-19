# VEC_MAPPING
This project aims at mapping high dimensional vectors to low dimensions by following https://github.com/artetxem/vecmap
## step1:
download the github repo from https://github.com/artetxem/vecmap
## step2:
download the source-vectors and source-vectors from here:
  - [source-vectors](https://cf-my.sharepoint.com/:t:/g/personal/wangy306_cardiff_ac_uk/EYIqLsCJvX9MvRoAIuohAdUB1u8ssWepmTExSSnaMRoHAA?e=4ZNJPZ)
  - [target-vectors](https://cf-my.sharepoint.com/:t:/g/personal/wangy306_cardiff_ac_uk/Eak7aUzkkCRNrz9MmgHawTkBzOURWFsFjsisT4-33N7z0Q?e=tLBo15)
  - [TRAIN.DICT](https://cf-my.sharepoint.com/:t:/g/personal/wangy306_cardiff_ac_uk/EcA06LRjl9ZAo38Qb7ST4eMBGsOYamsOgqJyRXco-OiRHw?e=6CK2KH)
## step3:
  - `python3 map_embeddings.py --supervised TRAIN.DICT SRC.EMB TRG.EMB SRC_MAPPED.EMB TRG_MAPPED.EMB`
  - TRAIN.DICT (if any, should be given as a text file with one entry per line (source word + whitespace + target word))
  - SRC.EMB and TRG.EMB (refer to the input monolingual embeddings, which should be in the word2vec text format)
  - SRC_MAPPED.EMB and TRG_MAPPED.EMB (refer to the output cross-lingual embeddings)
  - Command in this setting:`python3 map_embeddings.py --supervised ./mapping_dict.txt ./BERT_source.txt ./CBOW_target.txt ./BERT_mapped.txt ./CBOW_mapped.txt
`
