# Ichnaea-MST

**Ichnaea-MST** is an open-source software tool for *Microbial Source Tracking (MST)* that uses **machine learning** to identify the origin of faecal contamination in water. It is designed for microbiologists, environmental scientists, and water managers who want to apply advanced data analysis without programming expertise.

---

## What does Ichnaea-MST do?

Ichnaea-MST analyzes datasets containing microbial, viral, mitochondrial, and chemical markers to predict whether faecal pollution comes from **human or animal sources** (e.g. bovine, porcine, poultry).

The application:

* Trains machine learning models automatically
* Evaluates model performance
* Classifies new water samples
* Provides probabilistic results and clear performance metrics

---

## Key features

* **Automatic Machine Learning (AutoML)** powered by H2O
* Supports **binary and multi-class classification**
* Works with **quantitative and qualitative MST markers**
* Includes **data augmentation** to improve model robustness
* Optional **environmental decay (t90) correction** for sensitivity analysis
* Model interpretability tools (variable importance, ROC curves)

---

## How is it delivered?

Ichnaea-MST is available in two formats:

* **R Notebooks** for local execution in RStudio (advanced users)
* **Shiny Web Application** with a graphical user interface (no coding required)

Both versions share the same machine learning backend.

---

## Input data

The software accepts tabular files such as:

* CSV
* Excel (XLS/XLSX)
* ODS
* STATA / SPSS

Each dataset must include:

* A column defining the **contamination source (class)**
* Multiple columns with MST marker data
* Simple metadata indicating variable type and detection limits

---

## Typical workflow

1. Load the MST dataset
2. (Optional) Augment data by simulating dilution and detection limits
3. Train machine learning models using AutoML
4. Evaluate performance (accuracy, AUC, confusion matrix)
5. Classify new samples with probability estimates
6. Export results

---

## Outputs

* Best-performing trained model
* Classification probabilities for each sample
* Performance metrics and confusion matrices
* Variable importance plots

---

## Use cases

* Drinking water safety assessment
* Identification of faecal pollution sources in rivers and lakes
* Investigation of mixed-source contamination
* Support for regulatory monitoring and environmental management

---

## Limitations

* Model performance depends on the quality and representativeness of training data
* Results should be interpreted together with environmental and analytical context
* The decay correction is a simplified linear approximation

---

## License

Ichnaea-MST is released as **open-source software**. See the `LICENSE` file for details.

