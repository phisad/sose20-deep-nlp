# Final project

- The project can be done in groups of 1-3 people.  
- You need to hand in a group contract establishing the team members and
  evaluation conditions (if different from default).
- A list of possible topics will be provided, you can also choose your own topic
  but this must be approved by Sharid first.
- You need to hand in one written report per group.  
- By default, there will be a joint equal grade for all members of the group,
  based on the written group report. This default can be overwritten by the
  group contract.
- You have ~~three~~ five weeks after July 21st to complete your final project. The deadline is Friday ~~14th~~ August 28th, 2020, 11:00pm. 
  
## Project Proposal Guidelines

- TBD

## Written Report Guidelines

- Please use provided LaTeX template.  
- Length of 10 pages, references included.
- Be a good scholar, give credit where credit is due.  
- (Extra guidelines to be added later). 


## Late policy

- If you fail to meet the deadline, you can still submit your final report with
  a penalty of 2\% off your final grade per day. The report will not be
  accepted after 5 late working days. 
  
## Topics


### POS Tagging (less challenging)

This project is based on the paper

 	Plank et al. Multilingual Part-of-Speech Tagging with Bidirectional Long-Short Term Memory Models and Auxiliary Loss. ACL 2016

You should implement the BiLSTM tagging model described in the paper. If you want, you can skip the auxiliary loss part where the system predicts the frequency of input tokens. You should present experiments for UD v1.2 treebanks for English, German, and two additional languages of your choice. You can include additional languages if you want. If your results are not as good as the ones presented in the paper, try to figure out why this happens.

### Named-entity recognition (less challenging)

This project is based on the paper

    Lample et al. Neural Architectures for Named Entity Recognition. NAACL-HLT 2016.

You should implement a Bidirectional LSTM tagger (without the CRF layer described in the paper). You should compare your results on the CoNLL 2003 dataset to the results presented in the paper. If your system doesn't deliver as good performance as as the Lample et al. (2016) systems, try to figure out why that might be the case.

Link to CoNLL 2003 dataset: https://github.com/Franck-Dernoncourt/NeuroNER/tree/master/data/conll2003/en

### Word Inflection (moderately challenging)

This project is based on the paper

 	Kann and Schütze. MED: The LMU System for the SIGMORPHON 2016 Shared Task on Morphological Reinflection. SIGMORPHON 2016.

Your task is to implement the encoder-decoder system for word inflection described in the paper. You should train your system on the Finnish, German and Navajo datasets from the 2016 SIGMORPHON shared task on word inflection which can be found here: https://github.com/ryancotterell/sigmorphon2016/tree/master/data/

### Embeddings (moderately challenging)

This project is based on the paper

 	Bojanowski et al. Enriching Word Vectors with Subword Information. TACL 2017.

You should implement at least the negative sampling skipgram model for complete words described in Section 3.1. You can also include subword information if you want. You can use UD v 1.2 treebanks for German and English to train your word embeddings. You can present qualitative evaluation which shows that your model groups together semantically related words. You can also evaluate on the semantic similarity datasets used by Bojanowski et al. (2017) for German and English (GUR65, GUR350, ZG222, WS353, RW). This is, however, not required.

### Image Captioning (more challenging)

This project is based on the paper

 	Vinyals et al. Show and Tell: A Neural Image Caption Generator. CVPR 2015.

You should use one of the pretrained CNN image recognition models and the COCO dataset from torchvision: https://pytorch.org/docs/stable/torchvision/index.html On top of the recognition model, you should train an image captioning system which generates a caption sentence based on a representation vector computed by the CNN model.
