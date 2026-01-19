This document defines the Level 1 metamorphic test scenarios executed under a strict black-box assumption.  
All input variables (**A, B, C, D**) and the output (**E**) are treated as abstract system elements.

---

# **Scenario 1A: Assignment of Zero to Individual Inputs**

**Metamorphic Relation Type:** **Exclusive (E)**

### **Description**

In this scenario, the evaluator assesses the system’s sensitivity by assigning the value **zero** to exactly one abstract input variable at a time, while keeping all other inputs unchanged.

Each execution with modified data produces a **Metamorphic Prediction**, which is compared against the **Baseline Prediction** obtained from the unmodified reference dataset using quantitative metrics.

Assigning zero excludes the contribution of the selected input variable from the input vector. Observable deviations between the Baseline Prediction and the Metamorphic Prediction indicate that the excluded variable influences the system’s behavior under a strict black-box assumption.

---

### **Test Cases**

#### **CT_1A_001 — Exclusive Relation (A = 0)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **A** is assigned the value zero and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

#### **CT_1A_002 — Exclusive Relation (B = 0)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **B** is assigned the value zero and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

#### **CT_1A_003 — Exclusive Relation (C = 0)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **C** is assigned the value zero and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

#### **CT_1A_004 — Exclusive Relation (D = 0)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **D** is assigned the value zero and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

### **Evaluation Note**

These test cases evaluate whether excluding the contribution of a single abstract input variable leads to observable changes in the system output, indicating sensitivity under a strict black-box testing assumption.

---

# **Scenario 1B: Assignment of NULL to Individual Inputs**

**Metamorphic Relation Type:** **Exclusive (E)**

### **Description**

This scenario evaluates the system’s behavior when **NULL values** are assigned individually to abstract input variables.

Each test case removes one input variable from effective participation in the computation by replacing its value with NULL, while all other inputs remain unchanged.

The evaluator observes whether the system output changes, becomes undefined, or whether the execution is interrupted, indicating that the excluded variable interferes with the system’s operation.

---

### **Test Cases**

**CT_1B_001 — Exclusive Relation (A = NULL)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **A** is assigned the value **NULL** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** or execution behavior is compared against the **Baseline Prediction**.

---

**CT_1B_002 — Exclusive Relation (B = NULL)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **B** is assigned the value **NULL** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** or execution behavior is compared against the **Baseline Prediction**.

---

**CT_1B_003 — Exclusive Relation (C = NULL)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **C** is assigned the value **NULL** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** or execution behavior is compared against the **Baseline Prediction**.

---

**CT_1B_004 — Exclusive Relation (D = NULL)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **D** is assigned the value **NULL** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** or execution behavior is compared against the **Baseline Prediction**.

---

### **Evaluation Note**

These test cases evaluate how excluding the contribution of a single abstract input variable—by assigning a NULL value—affects the system output or interferes with execution, characterizing sensitivity to missing inputs under a strict black-box assumption.

---

# **Scenario 1C: Temporal Lag Applied to Individual Inputs**

**Metamorphic Relation Type:** **Permutative (P)**

### **Description**

In this scenario, the evaluator investigates the effect of **temporal reordering** applied to individual abstract input variables.

Each test case introduces a temporal lag of **10, 50, or 100 samples** to one input variable, while preserving the original ordering of the remaining inputs.

The transformation alters the alignment of samples without modifying their individual values, allowing the evaluator to observe whether temporal displacement of a single variable interferes with the system’s output behavior or execution.

---

### **Test Cases — Temporal Lag (lag = 10)**

**CT_1C_001 — Permutative Relation (A Lag = 10)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **A** is temporally shifted by **10 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

**CT_1C_002 — Permutative Relation (B Lag = 10)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **B** is temporally shifted by **10 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

**CT_1C_003 — Permutative Relation (C Lag = 10)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **C** is temporally shifted by **10 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

**CT_1C_004 — Permutative Relation (D Lag = 10)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **D** is temporally shifted by **10 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

### **Test Cases — Temporal Lag (lag = 50)**

**CT_1C_005 — Permutative Relation (A Lag = 50)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **A** is temporally shifted by **50 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

**CT_1C_006 — Permutative Relation (B Lag = 50)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **B** is temporally shifted by **50 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

**CT_1C_007 — Permutative Relation (C Lag = 50)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **C** is temporally shifted by **50 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

**CT_1C_008 — Permutative Relation (D Lag = 50)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **D** is temporally shifted by **50 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

### **Test Cases — Temporal Lag (lag = 100)**

**CT_1C_009 — Permutative Relation (A Lag = 100)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **A** is temporally shifted by **100 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

**CT_1C_010 — Permutative Relation (B Lag = 100)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **B** is temporally shifted by **100 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

**CT_1C_011 — Permutative Relation (C Lag = 100)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **C** is temporally shifted by **100 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

**CT_1C_012 — Permutative Relation (D Lag = 100)**  
**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **D** is temporally shifted by **100 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

### **Evaluation Note**

These test cases evaluate whether **temporal displacement of a single abstract input variable**, without modifying its values, interferes with the system’s output or execution behavior, revealing sensitivity to temporal dependencies under a strict black-box assumption.


# **Scenario 1D: Multiplicative Scaling of Individual Inputs**

**Metamorphic Relation Type:** **Multiplicative (M)**

### **Description**

This scenario evaluates how scaling the magnitude of individual abstract input variables affects the system output.

Each test case multiplies one input variable by a fixed factor (**×20**), while the remaining variables preserve their original values and structure.

The objective is to observe whether increasing the magnitude of a single input interferes with the system’s output or execution, while preserving proportional relationships within that variable.

---

### **Test Cases**

#### **CT_1D_001 — Multiplicative Relation (A × 20)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **A** is multiplied by **20** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

#### **CT_1D_002 — Multiplicative Relation (B × 20)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **B** is multiplied by **20** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

#### **CT_1D_003 — Multiplicative Relation (C × 20)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **C** is multiplied by **20** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

#### **CT_1D_004 — Multiplicative Relation (D × 20)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** input variable **D** is multiplied by **20** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

### **Evaluation Note**

These test cases assess whether amplifying the magnitude of a single abstract input variable, while preserving the structure of all others, interferes with the system’s output or execution behavior, characterizing sensitivity under a strict black-box assumption.
# **Scenario 1E: Gaussian Noise Injection into Individual Inputs**

**Metamorphic Relation Type:** **Sustainable (S)**

### **Description**

In this scenario, the evaluator analyzes the effect of injecting **Gaussian noise** into individual abstract input variables.

Each test case adds noise with moderate variance (**σ = 0.2**) to one input variable, while preserving the structure, dimensionality, and temporal organization of the dataset.

The objective is to observe whether localized stochastic perturbations interfere with the system output or disrupt execution, while maintaining the overall structure of the input data.

---

### **Test Cases**

#### **CT_1E_001 — Sustainable Relation (Gaussian Noise on A)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** Gaussian noise with **σ = 0.2** is added to input variable **A** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

#### **CT_1E_002 — Sustainable Relation (Gaussian Noise on B)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** Gaussian noise with **σ = 0.2** is added to input variable **B** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

#### **CT_1E_003 — Sustainable Relation (Gaussian Noise on C)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** Gaussian noise with **σ = 0.2** is added to input variable **C** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

#### **CT_1E_004 — Sustainable Relation (Gaussian Noise on D)**

**GIVEN** abstract input variables **A, B, C, and D**  
**WHEN** Gaussian noise with **σ = 0.2** is added to input variable **D** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction**.

---

### **Evaluation Note**

These test cases evaluate whether localized stochastic perturbations applied to individual abstract inputs interfere with the system’s output behavior or execution, while preserving the structural and temporal integrity of the input dataset, in accordance with the **Sustainable (S)** metamorphic relation.