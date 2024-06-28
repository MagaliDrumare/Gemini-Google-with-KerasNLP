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


### KerasNLP 
The latest Keras 3 machine learning framework lets you write and run your code in JAX, Pytorch, or Tensorflow. Learn about Gemma, the large language model family of open models from Google. We will teach you basic and advanced LLM workflows, including chat generation, LoRA fine-tuning, model parallelism to train on large-scale infrastructure, style alignment, model surgery, and more.
- https://youtu.be/TV7qCk1dBWA?feature=shared
new Keras + Hugging Face integration: you can now load HF fine-tuned models through Keras, even if they have not been fine-tuned in Keras. As long as the architecture is implemented in KerasNLP, weights will be converted on the fly.
- https://colab.research.google.com/drive/12_jhj36h5Ca_Le7jlU2PitFMBhQ83Si1?usp=sharing 
  

  

  
