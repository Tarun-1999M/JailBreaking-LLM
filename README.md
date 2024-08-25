# Jailbreaking Large Language Models (LLMs)

[![CCS: 2024](https://img.shields.io/badge/CCS-2024-red.svg)]()
[![license: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository focuses on the exploration and evaluation of jailbreak prompts on Large Language Models (LLMs). Inspired by the ACM CCS 2024 paper ["Do Anything Now'': Characterizing and Evaluating In-The-Wild Jailbreak Prompts on Large Language Models](https://arxiv.org/abs/2308.03825) by Xinyue Shen, Zeyuan Chen, Michael Backes, Yun Shen, and Yang Zhang, this project aims to extend the analysis with additional datasets and methodologies. 

The purpose of this project is to better understand the vulnerabilities of LLMs to adversarial prompts and to develop methods to mitigate these risks.

## Data

### Prompts

This project utilizes a dataset of 15,140 prompts collected from multiple platforms between December 2022 and December 2023. The prompts were sourced from forums, social media, and other online platforms, including Reddit, Discord, and open-source datasets. Among these, 1,405 prompts were identified as jailbreak prompts. The dataset is curated to explore the effectiveness of these prompts in bypassing safety mechanisms in LLMs.


| Platform  | Source                     | # Posts     | # UA      | # Adv UA | # Prompts  | # Jailbreaks | Prompt Time Range   |
| --------- | -------------------------- | ----------- | --------- | -------- | ---------- | ------------ | ------------------- |
| Reddit    | r/ChatGPT                  | 163549      | 147       | 147      | 176        | 176          | 2023.02-2023.11     |
| Reddit    | r/ChatGPTPromptGenius      | 3536        | 305       | 21       | 654        | 24           | 2022.12-2023.11     |
| Reddit    | r/ChatGPTJailbreak         | 1602        | 183       | 183      | 225        | 225          | 2023.02-2023.11     |
| Discord   | ChatGPT                    | 609         | 259       | 106      | 544        | 214          | 2023.02-2023.12     |
| Discord   | ChatGPT Prompt Engineering | 321         | 96        | 37       | 278        | 67           | 2022.12-2023.12     |
| Discord   | Spreadsheet Warriors       | 71          | 3         | 3        | 61         | 61           | 2022.12-2023.09     |
| Discord   | AI Prompt Sharing          | 25          | 19        | 13       | 24         | 17           | 2023.03-2023.04     |
| Discord   | LLM Promptwriting          | 184         | 64        | 41       | 167        | 78           | 2023.03-2023.12     |
| Discord   | BreakGPT                   | 36          | 10        | 10       | 32         | 32           | 2023.04-2023.09     |
| Website   | AIPRM                      | -           | 2777      | 23       | 3930       | 25           | 2023.01-2023.06     |
| Website   | FlowGPT                    | -           | 3505      | 254      | 8754       | 405          | 2022.12-2023.12     |
| Website   | JailbreakChat              | -           | -         | -        | 79         | 79           | 2023.02-2023.05     |
| Dataset   | AwesomeChatGPTPrompts      | -           | -         | -        | 166        | 2            | -                   |
| Dataset   | OCR-Prompts                | -           | -         | -        | 50         | 0            | -                   |
| **Total** |                            | **169,933** | **7,308** | **803**  | **15,140** | **1,405**    | **2022.12-2023.12** |




### Question Set

A comprehensive question set comprising 390 questions was constructed to evaluate the effectiveness of the identified jailbreak prompts. These questions are categorized into 13 forbidden scenarios as defined by the [OpenAI Usage Policy](https://openai.com/policies/usage-policies), including but not limited to Illegal Activity, Hate Speech, Malware Generation, and Privacy Violence.

## Methodology

The methodology of this project builds upon the foundational work presented in the original paper by Xinyue Shen and colleagues. Key enhancements and additional analyses are included to provide further insights into the robustness of LLMs against adversarial prompts.

### Key Components:

- **Prompt Evaluation**: The project assesses the impact of various jailbreak prompts on multiple LLMs, quantifying their ability to bypass built-in safeguards.
- **Semantic Analysis**: Advanced semantic visualization techniques are employed to understand the underlying patterns in the successful jailbreak prompts.
- **Evaluator Development**: Customized evaluators have been developed to automate the analysis of prompt effectiveness across different scenarios.


### Citation:
If you find this work useful, please consider citing the original authors of the dataset and the foundational research:

```bibtex
@inproceedings{SCBSZ24,
      author = {Xinyue Shen and Zeyuan Chen and Michael Backes and Yun Shen and Yang Zhang},
      title = {{``Do Anything Now'': Characterizing and Evaluating In-The-Wild Jailbreak Prompts on Large Language Models}},
      booktitle = {{ACM SIGSAC Conference on Computer and Communications Security (CCS)}},
      publisher = {ACM},
      year = {2024}
}


