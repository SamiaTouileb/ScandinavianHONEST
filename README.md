# Measuring Harmful Representations in Scandinavia Language Models

This repository contains the bias probes used and described in the paper ["*Measuring Harmful Representations in Scandinavian Language Models*"](https://arxiv.org/abs/2211.11678) by Samia Touileb and Debora Nozza, presented at the Fifth Workshop on Natural Lnagugae Processing and Computational Social Science, collocated with EMNLP 2022 in Abu Dhabi, Dec 7 2022.


# Abstract of the paper

Scandinavian countries are perceived as role-models when it comes to gender equality. With the advent of pre-trained language models and their widespread usage, we investigate to what extent gender-based harmful and toxic content exist in selected Scandinavian language models. We examine nine models, covering Danish, Swedish, and Norwegian, by manually creating template-based sentences and probing the models for completion. We evaluate the completions using two methods for measuring harmful and toxic completions and provide a thorough analysis of the results. We show that Scandinavian pre-trained language models contain harmful and gender-based stereotypes with similar values across all languages. This finding goes against the general expectations related to gender equality in Scandinavian countries and shows the possible problematic outcomes of using such models in real-world settings. 

# Replicating results

We used two measures to quantufy the harmful representation of the selected Scandinavian language models:

1. HONEST score: Following the work on (Nozza et al., 2021), we computed the HONEST scores using the python package available [*here*](https://github.com/MilaNLProc/honest). PLease refer to the following paper if you would like to know more about HONEST: Nozza D., Bianchi F., and Hovy D. "HONEST: Measuring hurtful sentence completion in language models." The 2021 Conference of the North American Chapter of the Association for Computational Linguistics: Human Language Technologies. Association for Computational Linguistics, 2021. https://aclanthology.org/2021.naacl-main.191

2. Toxic score: We used the [*perspective API*](https://perspectiveapi.com/) to compute the score. Check the paper for more details.  

# Additional results

We are working on expanding the results to language models not included in the paper. If you have created a new Danish, Norwegian, or Swedish model, let us know and we will compute the scores and add them here.

# Cite

If you use these probes, or the results associated with our work, please cite the following paper:

```
@misc{https://doi.org/10.48550/arxiv.2211.11678,
  doi = {10.48550/ARXIV.2211.11678},
  url = {https://arxiv.org/abs/2211.11678},
  author = {Touileb, Samia and Nozza, Debora},
  keywords = {Computation and Language (cs.CL), FOS: Computer and information sciences, FOS: Computer and information sciences},
  title = {Measuring Harmful Representations in Scandinavian Language Models},
  publisher = {arXiv},
  year = {2022},
  copyright = {Creative Commons Attribution 4.0 International}
}
```
