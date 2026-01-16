# Axiomatic Design Dataset

This repository releases a manually annotated dataset, curated by domain experts, and introduced in the following published work: 

*"Giordano, V., Consoloni, M., Losanno, M., Chiarello, F., & Fantoni, G. (2025). Decoding the grammar of design theory for large language models: the case of axiomatic design theory. Proceedings of the Design Society, 5, 1121–1130.* https://doi.org/10.1017/pds.2025.10126"

## Dataset Description

The dataset focuses on the annotation of Axiomatic Design (AXD) elements, specifically Functional Requirements (FRs) and Design Parameters (DPs), as defined in Suh’s Axiomatic Design theory (Suh, 2001).
For further details on the theory, see: https://www.axiomaticdesign.com/technology/axiomatic-design-advances-and-applications/

The dataset consists of 6,000 annotated sentences and it supports both sentence-level classification and word-level named entity recognition (NER) tasks.

### Sentence Classification
Each sentence is labeled according to its semantic content:
- **Functional**: Sentences describing only the functioning or behavior of the patented invention.
- **Structural**: Sentences describing only the architecture or structural aspects of the invention.
- **Mixed**: Sentences containing both functional and structural aspects.
- **Other**: Sentences that do not fall into the previous categories, typically including non-technical content such as contextual background or legal disclaimers.

### Named Entity Recognition (NER)
As illustrated in Fig. 1, the dataset includes token-level annotations for Axiomatic Design entities:
- **Doer**: The entity required to perform the action described in a FR.
- **Action**: The action of the FR that must be performed by the Doer.
- **Receiver**: The entity affected by the action.
- **Design Parameter (DP)**: A measurable attribute of a component that designers define and adjust within its feasible range to satisfy one or more functional requirements.

![Dataset Overview](https://github.com/Marco-Consoloni/axiomatic-design-dataset/blob/main/images/NER_annotation.png)

The annotations were conducted using [Doccano](https://doccano.github.io/doccano/), an open-source tool for text annotation that supports both entity and relation labeling.

### Repository Structure

#### `dataset/`
This folder contains the annotated dataset in two formats:
1. **`axiomatic_dataset.xlsx`**: Dataset in Excel format.
2. **`axiomatic_dataset_doccano.jsonl`**: For seamless import into the Doccano annotation tool.

#### `doccano_config/`
This folder includes the JSON configuration file for Doccano, defining:
- **`label_config_entity.json`**: configuration file for entity tags.
- **`label_config_rel.json`**: configuration file for relation tags.

### How to Use
1. Import `axiomatic_dataset_doccano.jsonl`file into [Doccano](https://doccano.github.io/doccano/) for visualization or further annotation.
2. Refer to the Excel file (`axiomatic_dataset.xlsx`) for tabular exploration of annotations.

### Contribute and Contact
We welcome contributions and feedback to enhance the dataset and its usability. Feel free to open issues or submit pull requests.
For questions or collaborations, reach out to **marco.consoloni@phd.unipi.it**.

