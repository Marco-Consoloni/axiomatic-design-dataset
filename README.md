# Axiomatic Design (AXD) Dataset

Paper Link:
[Link to Paper - To Be Added]

---

We are thrilled to release the **Axiomatic Design (AXD) Dataset**, a benchmark dataset consisting of:

- **6,000 sentences** annotated with **19,555 Axiomatic Design concepts**.
- **Validation** by domain experts.

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
1. Import the JSON dataset into [Doccano](https://doccano.github.io/doccano/) for visualization or further annotation.
2. Refer to the Excel file (`axiomatic_dataset.xlsx`) for tabular exploration of annotations.

---
### Contribute and Contact
We welcome contributions and feedback to enhance the dataset and its usability. Feel free to open issues or submit pull requests.
For questions or collaborations, reach out to [Marco Consoloni](marco.consoloni@phd.unipi.it).

