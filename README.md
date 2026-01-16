# Axiomatic Design (AXD) Dataset

This repository release a manual annotated dataset by domain experts that is constructed in the following published work: *Giordano, V., Consoloni, M., Losanno, M., Chiarello, F., & Fantoni, G. (2025). Decoding the grammar of design theory for large language models: the case of axiomatic design theory. Proceedings of the Design Society, 5, 1121-1130* https://doi.org/10.1017/pds.2025.10126."

We release a Datase which focus on the annotation of **Axiomatic Design (AXD)** technical concepts from Suh (2001) (https://www.axiomaticdesign.com/technology/axiomatic-design-advances-and-applications/), a benchmark dataset consisting of:

- **Sentence Classsification:** 6,000 sentences classified into four classes: **Functional, Structural, Mixed, and Other**.

- **Named Entity Recognition:** 6,000 sentences annotated with Functional Requirements (FRs) and Design Parameters (DPs) As illustrated in Figure 1

![Dataset Overview](https://github.com/Marco-Consoloni/axiomatic-design-dataset/blob/main/images/annotated_sentence_background.jpg)

The annotations were conducted using [Doccano](https://doccano.github.io/doccano/), an open-source tool for text annotation that supports both entity and relation labeling.

---

### Repository Structure

#### `dataset/`
This folder contains the annotated dataset in two formats:
1. **`axiomatic_dataset.xlsx`**: Dataset in Excel format.
2. **`axiomatic_dataset_doccano.jsonl`**: For seamless import into the Doccano annotation tool.

#### `doccano_config/`
This folder includes the JSON configuration file for Doccano, defining:
- **`label_config_entity.json`**: configuration file for entity tags.
- **`label_config_rel.json`**: configuration file for relation tags.

---

### How to Use
1. Import `axiomatic_dataset_doccano.jsonl`file into [Doccano](https://doccano.github.io/doccano/) for visualization or further annotation.
2. Refer to the Excel file (`axiomatic_dataset.xlsx`) for tabular exploration of annotations.

---
### Contribute and Contact
We welcome contributions and feedback to enhance the dataset and its usability. Feel free to open issues or submit pull requests.
For questions or collaborations, reach out to **marco.consoloni@phd.unipi.it**.

