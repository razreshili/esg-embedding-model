# esg-embedding-model
A master thesis project at TUM, which is focused on building a domain-adapted esg embedding model with contrastive learning training.

## Repository Structure

The repository is organized into the following folders:

### 1. `esg-domain`
- Contains notebooks for the ESG domain experiments.
    - **Dataset Creation :**
        -  Data_pairs_creation.ipynb : create a dataset with positive pairs using DeCLUTR (https://github.com/JohnGiorgi/DeCLUTR/tree/master)
        -  dataset_create_a_mix.ipynb : create a balanced dataset, where half of data is coming from adjacent positives and half is coming from subsuming positives. Also includes code for generating in-batch negatives
    - **Training :** train.ipynb <- fine-tuning models with PEFT techniques like LoRA, DoRA, and IA3 and using sentence-transformers trainer.

### 2. `medical-domain`
- Contains notebooks for the medical domain experiments.
    - **Dataset Creation and Training:** medical_Data_pairs_creation.ipynb, medical_dataset_create_a_mix.ipynb, and medical_train_notebook.ipynb are analagous to the notebooks in esg-domain folder, but adapted to medical datasets.
    - **Downstream dataset analysis:** medical_dataset.ipynb

### 3. `plots`
- Contains a notebook for generating visualizations.
    - **Plotting Notebook:** plot_10_sentences.ipynb <- plot 10 sentences (taken from BMW website) with model before and after contrastive training

### 4. `pre-processing`
- Contains a notebook for dataset filtering.
    - **Filtering Notebook:** merge_and_filter_data.ipynb
