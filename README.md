# Mathematic Optimization, Set-based Measures of Agreement, and Topic Model Alignment

Topic models are a class of unsupervised machine learning algorithms used to summarize the latent thematic content of an unstructured document collection. Topic models estimate a set of k=1…K latent topical vectors, characterized by semantically correlated words/tokens, that are used to summarize the thematic content of the document collection.  

Researchers are often interested in evaluating whether 1) ≥2 topic models fit to independent datasets yield similar thematic summarizations, or 2) ≥2 topic models fit to the same dataset, using different hyper-parameter configurations, yield similar thematic characterizations. Information from these analyses are used to assess the robustness and validity of unsupervised inferences generated via fitted topic models.    

A challenge with assessing semantic agreement of independent topic model fits relates to the permutation invariance of the estimated latent thematic matrices.  We propose using set-based measures of agreement (e.g. Jaccard’s coefficient and related metrics) to assess semantic agreement between thematic vectors. Optimal alignment of topic models fits is framed as a constrained integer programming/optimization problem . We illustrate how pyGurobi can be used to determine the optimal semantic alignment of two topic models fit to clinical note corpora collected from two independent primary care electronic medical record datasets. 

# Code contained in this repository were used:
- ASA/SDSS Conference, June 2024, Richmond (VA)
- MedArxiv pre-print

# Description of repository contents
- List of k=1...50 topical vectors describing the UTOPIAN primary care corpus (2017-2020, Toronto, Canada).
- List of k=1...50 topical vectors describing the EMRPC primary care corpus (2011-2015, Ontario, Canada).
- Jupyter Notebook to optimally align topical vectors using Jaccard coefficient as measure of agreement.
- Jupyter Notebook to optimally align topical vectors using set-intersection as measure of agreement.
- Jupyter Notebook to optimally align topical vectors using set-intersection of first-word/token as measure of agreement.

## UTOPIAN/EMRPC topic model fits
Additional details regarding the primary care topic models fit to the UTOPIAN/EMRPC datasets are provided in the folllowing manuscripts: 
- [Meaney et al. (2022). Non-negative matrix factorization temporal topic models and clinical text data identify COVID-19 pandemic effects on primary healthcare and community health in Toronto, Canada.][https://pubmed.ncbi.nlm.nih.gov/35202844/] 
- [Meaney et al. (2023). Comparison of Methods for Estimating Temporal Topic Models From Primary Care Clinical Text Data: Retrospective Closed Cohort Study.][https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9808604/]


