# Jailbreak Prompts on Large Language Models (LLMs)

## Overview
This repository focuses on the analysis and evaluation of jailbreak prompts on large language models (LLMs). Using the data provided by the [ACM CCS 2024 paper](https://github.com/Tarun-1999M/Jailbreaking-LLM) titled *"Do Anything Now: Characterizing and Evaluating In-The-Wild Jailbreak Prompts on Large Language Models"*, we explore the impact of these prompts across various LLMs.

## Data
### Prompts
Our dataset includes 15,140 prompts collected from multiple platforms between December 2022 and December 2023. This dataset, curated by Xinyue Shen, Zeyuan Chen, Michael Backes, Yun Shen, and Yang Zhang, is the largest collection of in-the-wild jailbreak prompts to date. 

| Platform  | Source                      | # Posts | # User Accounts | # Adversarial UAs | # Prompts | # Jailbreaks | Prompt Time Range |
|-----------|-----------------------------|---------|----------------|-------------------|-----------|--------------|-------------------|
| Reddit    | r/ChatGPT                   | 163,549 | 147            | 147               | 176       | 176          | 2023.02-2023.11   |
| Discord   | ChatGPT                     | 609     | 259            | 106               | 544       | 214          | 2023.02-2023.12   |
| Website   | FlowGPT                     | -       | 3,505          | 254               | 8,754     | 405          | 2022.12-2023.12   |
| Dataset   | AwesomeChatGPTPrompts       | -       | -              | -                 | 166       | 2            | -                 |
| **Total** |                             | 169,933 | 7,308          | 803               | 15,140    | 1,405        | 2022.12-2023.12   |

### Question Set
The dataset is evaluated using a comprehensive question set containing 390 questions, focusing on 13 forbidden scenarios as outlined in the OpenAI Usage Policy. These scenarios include Illegal Activity, Hate Speech, Malware Generation, and more.

## Methodology
Our approach builds upon the foundational data provided by the original authors. We employ advanced techniques to assess the effectiveness and robustness of jailbreak prompts across various large language models. This includes the use of customized evaluators, semantics visualization, and in-depth analysis of the collected data.

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


### Key Sections:
- **Overview:** Provide context about your project and the relationship to the original data.
- **Data:** Detail the dataset used, citing the original authors.
- **Methodology:** Describe your specific approach and any additional research or techniques you used.
- **Citation:** Properly credit the original authors, with the citation formatted in BibTeX.
- **License:** Ensure your repository is properly licensed.
- **Disclaimer:** Mention the nature of the data and its intended use.

This structure ensures that your README is clear, informative, and appropriately credits the original authors for their work while also explaining your contributions.
