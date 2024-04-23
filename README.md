# *A good pun is its own reword*: Can Large Language Models Understand Puns?

## Overview
Puns, as one of the common rhetorical devices, play a crucial role in the study of linguistics, particularly in the comprehensive analysis of linguistic humor. In this repository, we focus on three tasks—***pun recognition***, ***pun explanation***, and ***pun generation***—to systematically assess LLMs' capability of understanding puns. Our research uncovers the primary challenges faced when LLMs attempt to understand puns. More details are available in the corresponding [paper](https://arxiv.org/abs/2404.13599).

Our dataset merges two major public datasets on puns: the Semeval-2017-Task-7 dataset and the ExPun dataset. The former provides basic entries of puns and non-puns, while the latter augments the former with detailed human annotations (including explanations and keywords). These datasets are accessible at the following links:
* Semeval-2017-Task-7: [paper](https://aclanthology.org/S17-2005/), [dataset](https://alt.qcri.org/semeval2017/task7/index.php?id=data-and-resources)
* ExPun: [paper](https://aclanthology.org/2022.emnlp-main.304/), [dataset](https://github.com/amazon-science/expunations/tree/main/data)

## Experiment

### Prerequisites
* Setup environment: `pip install -r requirements.txt`
* Download the Semeval-2017-Task-7 and ExPun datasets (or directly use the processed data in the "dataset" folder)
* Add your API key in `_api_key.py`

### Code Description
* `1_build_dataset.ipynb`: integrate and process the original datasets to obtain examples and evaluation data
* `2_pun_recognition&explanation.ipynb`: call LLMs to recognize and explain puns
* `3_evaluation_of_recognition.ipynb`: evaluate the recognition results
* `4_evaluation_of_explanation.ipynb`: evaluate the explanation results
* `5_pun_generation.ipynb`: call LLMs to generate puns
* `6_evaluation_of_generation.ipynb`: evaluate the generation results

### Results
We have placed our experiment results in the "results" folder, which includes the LLMs' responses to the above three tasks and the corresponding evaluations.

## Citation
If you find this study useful for your methods, please cite the following paper:
```
@misc{xu2024a,
      title={"A good pun is its own reword": Can Large Language Models Understand Puns?}, 
      author={Zhijun Xu and Siyu Yuan and Lingjie Chen and Deqing Yang},
      year={2024},
      eprint={2404.13599},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```

