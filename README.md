# Few-Shot Classification for Hate Speech Detection

This repository is dedicated to showcasing the practical applications explored in the research "Few-Shot Classification for Hate Speech Detection". The primary motivation behind this study was to assess and validate the effectiveness of the Task-Aware Representation of Sentences (TARS) methodology, as described in the [original TARS paper](https://aclanthology.org/2020.coling-main.285.pdf), in the context of hate speech detection across multiple languages, using the XLM-RoBERTa model.

## Research Objectives

The research was driven by the following objectives:

1. **Evaluating TARS on Diverse Hate Speech Corpora**: To evaluate the effectiveness of TARS in handling semantically diverse and unbalanced hate speech datasets known for their complexity.

2. **Few-Shot and Zero-Shot Learning**: To explore the TARS framework's capacity for few-shot learning—making accurate predictions with limited labeled data—and zero-shot learning, inferring classifications for previously unseen labels.

3. **Knowledge Retention in TARS**: To investigate how well the TARS approach retains previously learned information when incorporating new labels and additional labeled data.

4. **TARS Performance Across Languages**: To assess TARS performance on hate speech datasets in various languages, including English, German, and Portuguese, thus exploring the method's multilingual capabilities.

## Repository Overview

The two Jupyter notebooks in this repository represent the final stage of a five-stage sequential training process using TARS methodology with a pretrained XLM-RoBERTa-base model.

### Process Overview

- **Stage Complexity**: The code samples are derived from the last stage of a complex process involving five distinct hate speech datasets.
- **Dataset Diversity**: These datasets spanned different languages (three in English, one in Brazilian Portuguese, and one in German) and varied in the number of categories, with minimal category overlap.
- **Model Training**: The pretrained XLM-RoBERTa-base model was employed, processing the data accordingly and modifying the classification layer to align with the TARS-method.
- **Sequential Training**: Throughout the training, we sequentially integrated all five datasets, evaluating the model's performance after each addition.
- **Learning Objectives**: The aim was to demonstrate the model's ability to learn new categories while retaining knowledge of previously learned ones.

### Final Stage Notebooks

- `model_training_final_step.ipynb`: This notebook illustrates the training process during the final stage.
- `EVAL_F1_all_datasets.ipynb`: This notebook evaluates the model's performance across all datasets after the final training stage.

### Visual Insights

Below are visual representations of the model's performance:

- **F1 Measure Evolution**: A graph showing F1 measures at each training step (Image to be attached).
- **Dataset Sizes and Composition**: An image depicting the size and proportion of positive examples in each dataset (Image to be attached).
- **Performance Comparison**: A graph comparing model performance on English datasets (steps 1,2, and 4) versus non-English datasets (steps 3 and 5), highlighting an interesting finding in multilingual model performance (Image to be attached).


## Visual Insights

Below are visual representations of the model's performance:

- **F1 Measure Evolution**: A graph showing F1 measures at each training step.

  <img src="images/F1%20Round%201%20-%20xlm-r%20-%20no%20freezing.png" width="60%" />
  <br><br>

- **Dataset Sizes and Composition**: An image depicting the size and proportion of positive examples in each dataset.
  
  <img src="images/Dataset%20sizes.png" width="60%" />
  <br><br>

- **Performance Comparison**: A graph comparing model performance on English datasets (steps 1,2, and 4) versus non-English datasets (steps 3 and 5), highlighting an interesting finding in multilingual model performance.
  
  <img src="images/F1%20Scores%20-%20Round%201%20-%20xlm-r%20--%20Step-avg%20for%20EN%20vs%20PT%20and%20DE%20datasets.png" width="60%" />
  <br><br>

## Contact for Full Research

For access to the full research and further inquiries, please contact me at [eugen.kaurov@gmail.com](mailto:eugen.kaurov@gmail.com).

## License

This research and the accompanying demonstrations are provided under the MIT License.
