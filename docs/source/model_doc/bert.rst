BERT
----------------------------------------------------

Overview
~~~~~~~~~~~~~~~~~~~~~

The BERT model was proposed in `BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding <https://arxiv.org/abs/1810.04805>`__
by Jacob Devlin, Ming-Wei Chang, Kenton Lee and Kristina Toutanova. It's a bidirectional transformer
pre-trained using a combination of masked language modeling objective and next sentence prediction
on a large corpus comprising the Toronto Book Corpus and Wikipedia.

The abstract from the paper is the following:

*We introduce a new language representation model called BERT, which stands for Bidirectional Encoder Representations
from Transformers. Unlike recent language representation models, BERT is designed to pre-train deep bidirectional
representations from unlabeled text by jointly conditioning on both left and right context in all layers. As a result,
the pre-trained BERT model can be fine-tuned with just one additional output layer to create state-of-the-art models
for a wide range of tasks, such as question answering and language inference, without substantial task-specific
architecture modifications.*

*BERT is conceptually simple and empirically powerful. It obtains new state-of-the-art results on eleven natural
language processing tasks, including pushing the GLUE score to 80.5% (7.7% point absolute improvement), MultiNLI
accuracy to 86.7% (4.6% absolute improvement), SQuAD v1.1 question answering Test F1 to 93.2 (1.5 point absolute
improvement) and SQuAD v2.0 Test F1 to 83.1 (5.1 point absolute improvement).*

Tips:

- BERT is a model with absolute position embeddings so it's usually advised to pad the inputs on
  the right rather than the left.
- BERT was trained with the masked language modeling (MLM) and next sentence prediction (NSP) objectives. It is efficient at predicting masked
  tokens and at NLU in general, but is not optimal for text generation.

The original code can be found `here <https://github.com/google-research/bert>`_.

BertConfig
~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertConfig
    :members:


BertTokenizer
~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertTokenizer
    :members: build_inputs_with_special_tokens, get_special_tokens_mask,
        create_token_type_ids_from_sequences, save_vocabulary


BertTokenizerFast
~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertTokenizerFast
    :members:


Bert specific outputs
~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.modeling_bert.BertForPretrainingOutput
    :members:


BertModel
~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertModel
    :members:


BertForPreTraining
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertForPreTraining
    :members:


BertForMaskedLM
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertForMaskedLM
    :members:


BertForNextSentencePrediction
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertForNextSentencePrediction
    :members:


BertForSequenceClassification
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertForSequenceClassification
    :members:


BertForMultipleChoice
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertForMultipleChoice
    :members:


BertForTokenClassification
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertForTokenClassification
    :members:


BertForQuestionAnswering
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.BertForQuestionAnswering
    :members:


TFBertModel
~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.TFBertModel
    :members:


TFBertForPreTraining
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.TFBertForPreTraining
    :members:


TFBertForMaskedLM
~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.TFBertForMaskedLM
    :members:


TFBertForNextSentencePrediction
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.TFBertForNextSentencePrediction
    :members:


TFBertForSequenceClassification
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.TFBertForSequenceClassification
    :members:


TFBertForMultipleChoice
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.TFBertForMultipleChoice
    :members:


TFBertForTokenClassification
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.TFBertForTokenClassification
    :members:


TFBertForQuestionAnswering
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. autoclass:: transformers.TFBertForQuestionAnswering
    :members:

