# esg-embedding-model
A master thesis project at TUM, which is focused on building a domain-adapted esg embedding model with contrastive learning training.

## Repository Structure

The repository is organized into the following folders:

### 1. `esg-domain`
- Contains Google Colab notebooks for the ESG domain experiments.
    - **Dataset Creation (2 Notebooks):** Preparation and preprocessing of the ESG-related dataset for contrastive learning.
    - **Training (1 Notebook):** Fine-tuning models with PEFT techniques like LoRA, DoRA, and IA3 for domain adaptation to ESG criteria.

### 2. `medical-domain`
- Contains Google Colab notebooks for the medical domain experiments.
    - **Dataset Creation (2 Notebooks):** Building and preprocessing a dataset from the medical field for contrastive learning.
    - **Training (1 Notebook):** Fine-tuning models with PEFT for domain-specific adaptation within the medical domain.

### 3. `plots`
- Contains a Google Colab notebook for generating visualizations.
    - **Plotting Notebook:** Generates plots of embeddings for a sample of 10 sentences from the BMW sustainability website, illustrating ESG-related representations.

### 4. `pre-processing`
- Contains one Google Colab notebook for initial dataset filtering.
    - **Filtering Notebook:** Defines the filtering criteria and methods used to process raw text data into clean, relevant samples for training and evaluation.
