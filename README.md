# re-evaluate-swipe
# Simplification Evaluation with Multiple Metrics

This repository provides code for evaluating text simplification using various metrics. 

## Dataset

The dataset `swipe_generator_data.json` originates from [Salesforce's Simplification repository](https://github.com/salesforce/simplification) and is licensed under the **Apache License 2.0**. This repository does not redistribute the original dataset but processes it into a different format for evaluation purposes.

## Repository Structure

- **`data_collection.ipynb`**: Converts `swipe_generator_data.json` into `input.csv`, which serves as the input for different evaluation metrics.
- **Evaluation Notebooks**:
  - `eval_with_len_salsa.ipynb`: Evaluates using LEN-SALSA.
  - `eval_with_questeval.ipynb`: Evaluates using QuestEval.
  - `eval_with_referee.ipynb`: Evaluates using Referee.
  - `eval_with_summac.ipynb`: Evaluates using SummaC.
- **`merged_data.ipynb`**: Merges the evaluation results from different metrics into a single dataset and and generating the final `evaluation_results.csv`.
- **`data/`**: Contains all generated evaluation inputs and outputs.

## Installation

Each evaluation notebook includes the necessary package installations. Ensure that you install the required dependencies before running the notebooks.

## Usage

1. Run `data_collection.ipynb` to generate `input.csv`.
2. Execute any of the evaluation notebooks to obtain metric-based evaluations.
3. Use `merged_data.ipynb` to combine all evaluation results.

## License

This project is licensed under the **Apache License 2.0**. See the [LICENSE](LICENSE) file for details.

### Acknowledgment
The dataset used in this project is sourced from [Salesforce’s Simplification repository](https://github.com/salesforce/simplification) and follows the **Apache License 2.0**.
