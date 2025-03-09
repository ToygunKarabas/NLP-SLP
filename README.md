# Natural Language Processing / Spoken Language Processing Project

## Dataset

FLEURS (Few-shot Learning Evaluation of Universal Representations of Speech) is a dataset for evaluating speech recognition systems in 102 languages, including many that are classified as 'low-resource'. The data is derived from the FLoRes-101 dataset, a machine translation corpus with 3001 sentence translations from English to 101 other languages. Native speakers are recorded narrating the sentence transcriptions in their native languages. The recorded audio data is paired with a label for the language in which it is spoken. The dataset can be used as an audio classification dataset for language identification: systems are trained to predict the language of each utterance in the corpus.

Dataset huggingface: https://huggingface.co/datasets/WueNLP/sib-fleurs

SIB-Fleurs is a dataset suitable to evaluate Multilingual Spoken Language Understanding. For each utterance in Fleurs, the task is to determine the category the utterance belongs to. The categories are:

* Science/Technology

* Travel

* Politics

* Sports

* Health

* Entertainment

* Geography

From this dataset 5 languages are selected: 

* Turkish

* English

* Spanish

* French

* German

## What has been done

1. Preliminary analysis with **nltk** & **spacy**

2. Speech recognition & Audio transcription with **SpeechRecognition** & **pydub**

3. Text preprocessing & vectorization with **spacy** & **huggingface** (construct datasets.ipynb)

4. Building category prediction pipelines from preprocessed texts using **sklearn**

    4.1. Hyperparameter tuning with **sklearn**

5. Building category prediction pipelines from preprocessed texts using **pytorch**

    5.1. Hyperparameter tuning with **Optuna**

    5.2. Hyperparameter tuning with **Skorch & sklearn**

    5.3. Hyperparameter tuning with **Ray Tune**

6. Performances reports & observations