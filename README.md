# Gemini-

Gemma is a family of lightweight, state-of-the art open models built from the same research and technology used to create the Gemini models.

Large Language Models (LLMs) like Gemma have been shown to be effective at a variety of NLP tasks. An LLM is first pre-trained on a large corpus of text in a self-supervised fashion. Pre-training helps LLMs learn general-purpose knowledge, such as statistical relationships between words. An LLM can then be fine-tuned with domain-specific data to perform downstream tasks (such as sentiment analysis).

LLMs are extremely large in size (parameters in the order of billions). Full fine-tuning (which updates all the parameters in the model) is not required for most applications because typical fine-tuning datasets are relatively much smaller than the pre-training datasets.

Low Rank Adaptation (LoRA){:.external} is a fine-tuning technique which greatly reduces the number of trainable parameters for downstream tasks by freezing the weights of the model and inserting a smaller number of new weights into the model. This makes training with LoRA much faster and more memory-efficient, and produces smaller model weights (a few hundred MBs), all while maintaining the quality of the model outputs.

This tutorial walks you through using KerasNLP to perform LoRA fine-tuning on a Gemma 2B model using the Databricks Dolly 15k dataset{:.external}. This dataset contains 15,000 high-quality human-generated prompt / response pairs specifically designed for fine-tuning LLMs.

### Getting started with Gemini 
- https://github.com/GoogleCloudPlatform/generative-ai/tree/main/gemini/getting-started

### Gemini avec Vertex AI 
- Accès la console Google Cloud  : https://accounts.google.com/
- Créer un projet pour obtenir l'ID projet / lancer la console si nécessaire 
- Rentrer ID du projet dans code Google Colab
- Supprimer le projet dans la console Google Cloud 


### Gemma: Introducing new state-of-the-art open models
-https://blog.google/technology/developers/gemma-open-models/
- Accès à Gemma dans Kaagle : https://www.kaggle.com/models/google/gemma
- Générer un jeton API dans Kaagle pour télécharger le modèle dans Google Colab : https://www.kaggle.com/settings
- Dans Google Colab rubrique secrets mettre les éléments générer par l'API Kaagle KAGGLE_USERNAME : XXXXXXXXXXXX , KAGGLE_KEY: XXXXXXXXXXX (voir copie écran) 
- Large language models with Keras : https://youtu.be/TV7qCk1dBWA?feature=shared
- Chargement gemma_2b_en avec config Colab T4 GPU / memoire RAM élevée
  

  

  
