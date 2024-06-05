# TruthEval: A Dataset to Evaluate LLM Truthfulness and Reliability.

## Authors: 
Aisha Khatun and Daniel G. Brown. 

David R. Cheriton School of Computer Science. 

University of Waterloo, Canada.

## Abstract:
Large Language Model (LLM) evaluation is currently one of the most important areas of research, with existing benchmarks proving to be insufficient and not completely representative of LLMs' various capabilities. We present a curated collection of challenging statements on sensitive topics for LLM benchmarking called TruthEval. These statements were curated by hand and contain known truth values. The categories were chosen to distinguish LLMs' abilities from their stochastic nature. We perform some initial analyses using this dataset and find several instances of LLMs failing in simple tasks showing their inability to understand simple questions.

## Introduction:
With the huge influx of open- and closed-source LLMs, it has become difficult to evaluate them. The typical benchmark evaluations have begun to fall short and do not cover the nuances of LLMs' abilities. Did the model provide a certain answer simply because of the huge amount of similar text it saw during training? Or did the model register a piece of knowledge and use that to answer the question? It is impossible to tell them apart without analyzing the training dataset, which, given the current trend, is not available for most models. Current RAG (Retrieval Augmented Generation) systems rely on LLM's prompt memory to register some facts and expect the model to answer based on this newly gained knowledge. Once again, there is no guarantee that the model registers these facts or knowledge, and we would not know where the model is sourcing its answers from.

Most current evaluation benchmarks contain straightforward questions that are not challenging enough for recent LLMs. Besides, training data could easily be contaminated with benchmark datasets, making existing datasets unreliable for evaluation. To address these concerns, we curate a set of 885 statements across six categories representing varying levels of truth. This allows us to identify parrots from the usable models. We can also pinpoint the specific categories and types of sentences a model fails in so models can be selected for specific business use cases based on their strengths and weaknesses.

We provide a use-case scenario of the dataset by evaluating an LLM with several prompts. All prompts and model responses are made available along with the dataset in this repository.

## Cite:
```
@misc{khatun2024trutheval,
      title={TruthEval: A Dataset to Evaluate LLM Truthfulness and Reliability}, 
      author={Aisha Khatun and Daniel G. Brown},
      year={2024},
      eprint={2406.01855},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```

