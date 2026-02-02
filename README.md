# Metamorphic Tests

This repository contains the experimental artifacts of **Metamorphic Testing** developed in the context of the scientific research presented in the article:

> **“Metamorphic Testing for Machine Learning Based Measuring Systems.”**

This research was authored by **P. E. S. Santos, J. A. C. Braz, R. P. David, and W. S. Melo Jr.**, conducted in collaboration with:

- National Institute of Metrology, Quality and Technology (Inmetro), Brazil  
- iLAB – Software Quality Assurance  

The repository supports the execution, organization, and analysis of experiments, enabling test reproducibility and the systematic evaluation of results obtained at different levels of complexity, particularly in the context of **black-box evaluation of machine learning–based measuring systems within Legal Metrology**.

---

## 1. Scientific Context and Foundational Work

The experiments conducted in this repository derive from and extend the work made available by the Conect2AI research group, as described in the following repository and scientific article:

- **Base repository (original system):**  
  https://github.com/conect2ai/MDPI2023-pollution  

- **Associated scientific article:**  
  https://www.mdpi.com/2071-1050/16/2/708  

- **Conect2AI research group:**  
  https://www.instagram.com/conect2ai  

---

## 2. System Under Test (SUT)

The **System Under Test (SUT)** used in the Metamorphic Testing experiments corresponds to the set of notebooks, predictive models, and simulations available in the previously mentioned base repository.

This system includes:

- Vehicular trip data analysis  
- Predictive models for variables used in emission calculations  
- Simulations based on SUMO and urban graph networks  

The SUT serves as the foundation for defining, applying, and evaluating the metamorphic relations investigated in this research.

---

## 3. Organization of Metamorphic Tests

The Metamorphic Tests were organized into increasing levels of complexity according to the experimental design presented in the article and were implemented in independent Jupyter notebooks:

- `Level_1_metamorphic_tests.ipynb`
- `Level_2_metamorphic_tests.ipynb`
- `Level_3_metamorphic_tests.ipynb`

Each notebook includes:

- Definition of metamorphic test cases  
- Application of metamorphic relations  
- Execution of tests over the SUT  
- Collection and analysis of metrics per test case  

---

## 4. Metamorphic Test Plans

The **Metamorphic Test Plans** are documented in the `metamorphic_test_plans/` folder and describe, in a structured manner, the planning of the tests executed at each experimental level.

**Available files:**

- `Test_Plan_Level_1.md`
- `Test_Plan_Level_2.md`
- `Test_Plan_Level_3.md`

Each test plan presents:

- The objective of the test level  
- The characterization of the applied metamorphic relations  
- The execution strategy for the test cases  
- The traceability link between planned tests and execution notebooks  

These documents formalize the experimental design of the Metamorphic Tests, ensuring traceability, methodological clarity, and support for reproducibility.

---

## 5. Notebooks Derived from the Original System

The notebooks listed below were not specifically developed for Metamorphic Testing but are part of the original system under test and are used to support the execution of the experiments:

- `initial_analysis.ipynb`
- `predict_maf.ipynb`
- `predict_afr.ipynb`
- `predict_co2.ipynb`
- `predict_maf_lightweight.ipynb`
- `predict_afr_lightweight.ipynb`
- `simulate_sumo.ipynb`
- `create_graph_network.ipynb`

These notebooks were originally developed within the base repository and are maintained in this repository exclusively for the purpose of reproducing the system under test. They do not constitute Metamorphic Testing artifacts.

The separation between the system under test and the testing artifacts ensures methodological clarity and experimental validity.

---

## 6. Experimental Results

The consolidated results of the experiments are available in the `results/` folder in **PDF format**, containing:

- Graphs generated during test execution  
- Metrics obtained per metamorphic test case  
- Results organized by test level  

**Available files:**

- `L1 - Metamorphic Test Cases.pdf`
- `L2 - Metamorphic Test Cases.pdf`
- `L3 - Metamorphic Test Cases.pdf`

---

## 7. Experimental Environment and Reproducibility

The dependencies and execution environment of the experiments are described in the following files:

- `requirements.txt`
- `environment.yml`

These files enable the reproduction of the experimental environment adopted in this research.

---

## 8. Academic Context

The materials made available in this repository aim to:

- Support the reproducibility of the experiments described in the article  
- Facilitate comparative analysis across different levels of Metamorphic Testing  
- Serve as a foundation for future studies in the field of Software Quality and Testing of Machine Learning–Based Systems  

This repository is intended exclusively for academic and scientific purposes.
