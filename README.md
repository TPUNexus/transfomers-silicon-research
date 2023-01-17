# BERT Model on Silicon
> **Research and Materials on Hardware implementation of BERT (Bidirectional Encoder Representations from Transformers) Model**

## BERT Model

### Description
BERT is a method of pre-training language representations, meaning that we train a general-purpose "language understanding" model on a large text corpus (like Wikipedia) and then use that model for downstream NLP tasks. BERT was created and published in 2018 by Jacob Devlin and his colleagues from Google. BERT is conceptually simple and empirically powerful. It obtains new state-of-the-art results on eleven natural language processing tasks, including pushing the GLUE score to 80.5% (7.7% point absolute improvement), MultiNLI accuracy to 86.7 (5.6% absolute improvement), SQuAD v1.1 question answering Test F1 to 93.2 (1.5% absolute improvement) and SQuAD v2.0 Test F1 to 83.1 (5.1% absolute improvement).

### Architecture

BERT is a Transformer-based model. The architecture of BERT is similar to the original Transformer model, except that BERT has two separate Transformer models: one for the left-to-right direction (the “encoder”) and one for the right-to-left direction (the “encoder”). The output of each model is the hidden state output by the final Transformer layer. The two models are pre-trained jointly on a large corpus of unlabeled text. The pre-training task is a simple and straightforward masked language modeling objective. The pre-trained BERT model can then be fine-tuned with just one additional output layer to create state-of-the-art models for a wide range of tasks, such as question answering and language inference, without substantial task-specific architecture modifications.

--- 

## Reference Papers

**1. Attention Is All You Need**

 [![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/1706.03762) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/1706.03762.pdf) [![Code-Link](https://img.shields.io/badge/Code-PyTorch-red?style=plastic)](https://github.com/jadore801120/attention-is-all-you-need-pytorch) [![Code-Link](https://img.shields.io/badge/Code-TensorFlow-orange?style=plastic)](https://github.com/lsdefine/attention-is-all-you-need-keras)
 
<details>
<summary><img src="https://img.shields.io/badge/ABSTRACT-9575cd?&style=plastic"/></summary>
The dominant sequence transduction models are based on complex recurrent or convolutional neural networks that include an encoder and a decoder. The best performing models also connect the encoder and decoder through an attention mechanism. We propose a new simple network architecture, the Transformer, based solely on attention mechanisms, dispensing with recurrence and convolutions entirely. Experiments on two machine translation tasks show these models to be superior in quality while being more parallelizable and requiring significantly less time to train. Our model achieves 28.4 BLEU on the WMT 2014 Englishto-German translation task, improving over the existing best results, including ensembles, by over 2 BLEU. On the WMT 2014 English-to-French translation task, our model establishes a new single-model state-of-the-art BLEU score of 41.8 after training for 3.5 days on eight GPUs, a small fraction of the training costs of the best models from the literature. We show that the Transformer generalizes well to other tasks by applying it successfully to English constituency parsing both with large and limited training data.
</details>

#

**2. BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding**

 [![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/1810.04805) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/1810.04805.pdf) [![Code-Link](https://img.shields.io/badge/Code-TensorFlow-orange?style=plastic)](https://github.com/google-research/bert) [![Code-Link](https://img.shields.io/badge/Code-PyTorch-red?style=plastic)](https://github.com/codertimo/BERT-pytorch) 

<details>
<summary><img src="https://img.shields.io/badge/ABSTRACT-9575cd?&style=plastic"/></summary>
We introduce a new language representation model called BERT, which stands for
Bidirectional Encoder Representations from Transformers. Unlike recent language representation models (Peters et al., 2018a; Radford et al., 2018), BERT is designed to pretrain deep bidirectional representations from unlabeled text by jointly conditioning on both left and right context in all layers. As a result, the pre-trained BERT model can be finetuned with just one additional output layer to create state-of-the-art models for a wide range of tasks, such as question answering and language inference, without substantial taskspecific architecture modifications.
<br>
BERT is conceptually simple and empirically powerful. It obtains new state-of-the-art results on eleven natural language processing tasks, including pushing the GLUE score to 80.5% (7.7% point absolute improvement), MultiNLI accuracy to 86.7% (4.6% absolute
improvement), SQuAD v1.1 question answering Test F1 to 93.2 (1.5 point absolute improvement) and SQuAD v2.0 Test F1 to 83.1 (5.1 point absolute improvement).
</details>

## Important Papers

**Distilling the Knowledge in a Neural Network, 2015**
[![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/1503.02531) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/1503.02531.pdf)


**Distilling Knowledge Learned in BERT for Text Generation, 2020**
[![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs//1911.03829) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/1911.03829.pdf)


**DistilBERT, a distilled version of BERT: smaller, faster, cheaper and lighter, 2019**
[![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/1910.01108) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/1910.01108.pdf)

**TinyBERT: Distilling BERT for Natural Language Understanding, 2020**
[![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/1909.10351) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/1909.10351.pdf)

**Distilling the Knowledge in a Neural Network, 2015**
[![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/1503.02531) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/1503.02531.pdf)

**FastBERT: a Self-distilling BERT with Adaptive Inference Time, 2020**
[![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/2004.02178) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/2004.02178.pdf)

**Distilling Task-Specific Knowledge from BERT into Simple Neural Networks, 2019**
[![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/1903.12136) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/1903.12136.pdf)

**Patient Knowledge Distillation for BERT Model Compression, 2019**
[![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/1908.09355) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/1908.09355.pdf)

**MobileBERT: a Compact Task-Agnostic BERT for Resource-Limited Devices, 2020**
[![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/2004.02984) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/2004.02984.pdf)

**Improving Multi-Task Deep Neural Networks via Knowledge Distillation for Natural Language Understanding, 2019**
[![Paper-Link](https://img.shields.io/badge/Paper-Link-blue?&style=plastic)](https://arxiv.org/abs/1904.09482) [![PDF-Download](https://img.shields.io/badge/PDF-Download-green?logoColor=red&&style=plastic&logo=adobe)](https://arxiv.org/pdf/1904.09482.pdf)

