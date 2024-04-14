# Fintune Sentence Transformer Using SetFit

## SetFit with sentence-transformers/LaBSE

This is a [SetFit](https://github.com/huggingface/setfit) model that can be used for Text Classification. This SetFit model uses [sentence-transformers/LaBSE](https://huggingface.co/sentence-transformers/LaBSE) as the Sentence Transformer embedding model. A [LogisticRegression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html) instance is used for classification.

The model has been trained using an efficient few-shot learning technique that involves:

1. Fine-tuning a [Sentence Transformer](https://www.sbert.net) with contrastive learning.
2. Training a classification head with features from the fine-tuned Sentence Transformer.

## Model Details

### Model Description
- **Model Type:** SetFit
- **Sentence Transformer body:** [sentence-transformers/LaBSE](https://huggingface.co/sentence-transformers/LaBSE)
- **Classification head:** a [LogisticRegression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html) instance
- **Maximum Sequence Length:** 256 tokens
- **Number of Classes:** 4 classes
- **Training Dataset:** [SumArabic](https://data.mendeley.com/datasets/7kr75c9h24/1)
- **Language:** Arabic

### Model Sources

- **Repository:** [SetFit on GitHub](https://github.com/huggingface/setfit)
- **Paper:** [Efficient Few-Shot Learning Without Prompts](setfit.pdf)
- **Blogpost:** [SetFit: Efficient Few-Shot Learning Without Prompts](https://huggingface.co/blog/setfit)
- **Model** [Ezzaldin-97/LaBSE-based-Arabic-News-Classifier](https://huggingface.co/Ezzaldin-97/LaBSE-based-Arabic-News-Classifier)