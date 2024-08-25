# Jailbreak Prompts on Large Language Models (LLMs)

## Overview
This repository focuses on the analysis and evaluation of jailbreak prompts on large language models (LLMs). Using the data provided by the [ACM CCS 2024 paper](https://github.com/Tarun-1999M/Jailbreaking-LLM) titled *"Do Anything Now: Characterizing and Evaluating In-The-Wild Jailbreak Prompts on Large Language Models"*, we explore the impact of these prompts across various LLMs.

## Data
### Prompts
Our dataset includes 15,140 prompts collected from multiple platforms between December 2022 and December 2023. This dataset, curated by Xinyue Shen, Zeyuan Chen, Michael Backes, Yun Shen, and Yang Zhang, is the largest collection of in-the-wild jailbreak prompts to date. 

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
The dataset is evaluated using a comprehensive question set containing 390 questions, focusing on 13 forbidden scenarios as outlined in the OpenAI Usage Policy. These scenarios include Illegal Activity, Hate Speech, Malware Generation, and more.

## Methodology
Our approach builds upon the foundational data provided by the original authors. We employ advanced techniques to assess the effectiveness and robustness of jailbreak prompts across various large language models. This includes the use of customized evaluators, semantics visualization, and in-depth analysis of the collected data.

## License
This repository is licensed under the MIT License. See the LICENSE file for more details.

## Citation
This work builds on the data and research conducted by Xinyue Shen, Zeyuan Chen, Michael Backes, Yun Shen, and Yang Zhang. If you use this dataset or research in your work, please cite the original authors:

```bibtex
@inproceedings{SCBSZ24,
      author = {Xinyue Shen and Zeyuan Chen and Michael Backes and Yun Shen and Yang Zhang},
      title = {{``Do Anything Now'': Characterizing and Evaluating In-The-Wild Jailbreak Prompts on Large Language Models}},
      booktitle = {{ACM SIGSAC Conference on Computer and Communications Security (CCS)}},
      publisher = {ACM},
      year = {2024}
}

