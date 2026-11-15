# CpG Island Region Benchmark

CpG islands are regions of DNA where a cytosine followed by a guanine (CpG) occurs more often than in the surrounding sequence. This study compares methods for finding these regions in the human reference genome (hg38). It evaluates a neural network, a LightGBM model, and seven classical methods. We use UCSC CpG island annotations to assess how well the methods identify individual DNA windows, detect whole islands, and locate their start and end positions.

## Data, code, and results

Download the numbered ZIP files from [release v1.0.0](https://github.com/YounisAnis/cpg-island-region-benchmark/releases/tag/v1.0.0). Extract them into the same directory to keep related files together.

| Archive                           | What it contains                                                                                     |
| --------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `01_Dataset.zip`                | Reference annotations, 200-base-pair training, validation, and test windows, and sampling summaries. |
| `02_Code_Environment.zip`       | Research code, Python requirements, and software environment details.                                |
| `03_Models_Configurations.zip`  | Trained models and settings for the primary models.                                                  |
| `04_Primary_Analysis.zip`       | Window and region results, predicted islands, boundary errors, and figures.                          |
| `05_Comparator_Analysis.zip`    | Settings and results for the seven classical methods.                                                |
| `06_Controlled_Experiments.zip` | Models, training histories, and results for 27 runs comparing window sizes and model components.     |
| `07_Documentation.zip`          | Study overview, data sources, methods, and limitations.                                              |

After extraction, `Dataset/` holds the data, `Code/` holds the scripts, and `Models/` holds the trained models. Results are in `Analysis/`, study notes are in `Documentation/`, and configuration and provenance details are in `Metadata/`. To find a specific file, look up its name in the release asset `source_manifest.csv`.

## Author and supervisor

| Role       | Name        | Email                 |
| ---------- | ----------- | --------------------- |
| Author     | Younis Anis | younasanis6@gmail.com |
| Supervisor | Dr Shujaat  | shujaat@jbnu.ac.kr    |
