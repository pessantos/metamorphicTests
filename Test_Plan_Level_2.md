This document defines the Level 2 metamorphic test scenarios, in which the evaluator possesses semantic knowledge of the input variables and evaluates whether the system’s output behavior remains causally coherent under physically, spatially, and temporally meaningful transformations

## **Scenario 2A — Multiplicative Scaling of Kinematic Inputs**

**Metamorphic Relation Type:** **Multiplicative (M)**
### **Description**

This scenario evaluates the system’s causal coherence when **kinematic input variables** are scaled by fixed multiplicative factors.

Each test case applies a multiplicative transformation to one or more kinematic variables—**Speed** and **Acceleration**—while preserving the remaining inputs (**Latitude** and **Longitude**), the dataset structure, and temporal ordering.

According to the **Multiplicative (M)** metamorphic relation, scaling input magnitudes is expected to induce **proportional and coherent variations** in the system output, without interrupting execution or violating internal consistency.

The resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** using quantitative metrics and visual inspection.

---

### **Test Cases**

---

#### **CT_2A_001 — Multiplicative Relation (Speed ×20)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** input variable **Speed** is multiplied by **20** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to assess proportional output variation.

---

#### **CT_2A_002 — Multiplicative Relation (Speed ×40)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** input variable **Speed** is multiplied by **40** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to assess proportional output variation.

---

#### **CT_2A_003 — Multiplicative Relation (Speed & Acceleration ×10)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** both **Speed** and **Acceleration** are multiplied by **10** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to evaluate causal coherence under joint scaling.

---

#### **CT_2A_004 — Multiplicative Relation (Speed & Acceleration ×20)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** both **Speed** and **Acceleration** are multiplied by **20** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to evaluate proportional and consistent output behavior.

---

#### **CT_2A_005 — Multiplicative Relation (Speed & Acceleration ×30)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** both **Speed** and **Acceleration** are multiplied by **30** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to assess scalability limits and causal consistency.

---

### **Evaluation Note**

These test cases assess whether the system output responds **coherently and proportionally** to multiplicative changes in kinematic inputs, as prescribed by the **Multiplicative (M)** metamorphic relation. Non-proportional responses, execution failures, or incoherent output trends are interpreted as potential violations of causal consistency at **Metamorphic Test Level 2**.

---

## **Scenario 2B — Additive Translation of Spatial Coordinates**

**Metamorphic Relation Type:** **Additive (A)**

### **Description**

This scenario evaluates the system’s causal and spatial coherence when **constant additive translations** are applied to spatial input variables.

Each test case applies a fixed additive offset to the spatial coordinates (**Latitude** and **Longitude**), while preserving all other input variables, the temporal structure, and the dynamic relationships among samples.

According to the **Additive (A)** metamorphic relation, spatial translations that do not alter relative positions or motion dynamics are expected to produce **minimal or structurally consistent variations** in the system output. Significant deviations may indicate sensitivity to absolute spatial positioning rather than relative spatial relationships.

The resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** using quantitative metrics and visual inspection.

---
### **Test Cases**

---
### **CT_2B_001 — Additive Relation (Coordinate Translation +1.0)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** **Latitude** and **Longitude** are increased by a constant offset of **+1.0** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to assess spatial invariance and output coherence.

---

### **CT_2B_002 — Additive Relation (Coordinate Translation +5.0)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** **Latitude** and **Longitude** are increased by a constant offset of **+5.0** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to evaluate the effect of larger spatial translations on system behavior.

---

### **Evaluation Note**

These test cases assess whether the system output remains **coherent and structurally consistent** under constant spatial translations, as prescribed by the **Additive (A)** metamorphic relation. Disproportionate output changes, execution failures, or loss of signal structure are interpreted as potential violations of spatial invariance at **Metamorphic Test Level 2**
    

---


## **Scenario 2C — Directional Inversion of Dynamic Input**

**Metamorphic Relation Type:** **Inversive (IV)**

### **Description**

This scenario evaluates the system’s causal coherence when the **direction of a dynamic input variable** is inverted.

The test case applies a **sign inversion** to the **Acceleration** variable, transforming positive values into negative ones and vice versa, while preserving the magnitude, temporal structure, and all remaining input variables.

According to the **Inversive (IV)** metamorphic relation, directional inversion is expected to induce **perceptible and coherent changes** in the system output, reflecting sensitivity to directional dynamics without causing execution failures or structural inconsistencies.

The resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** using quantitative metrics and visual inspection.

---

### **Test Cases**

---
#### **CT_2C_001 — Inversive Relation (Acceleration Sign Inversion)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** the sign of the **Acceleration** variable is inverted and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to assess directional sensitivity and causal coherence.

---

### **Evaluation Note**

This test case evaluates whether the system output responds **consistently and meaningfully** to the inversion of a directional dynamic input, as required by the **Inversive (IV)** metamorphic relation. Absence of observable change, erratic behavior, or execution failure is interpreted as a potential violation of directional coherence at **Metamorphic Test Level 2**.
    

---

## **Scenario 2D — Temporal Reordering of Speed Signal**

**Metamorphic Relation Type:** **Permutative (P)**

### **Description**

This scenario evaluates the system’s sensitivity to **temporal reordering** applied to a single kinematic input variable.

Each test case introduces a **temporal lag** to the **Speed** signal, shifting its samples forward in time while preserving the original values, dataset structure, and all remaining input variables.

According to the **Permutative (P)** metamorphic relation, reordering samples without modifying their individual values is expected to produce **progressive and coherent variations** in the system output as the temporal displacement increases, without interrupting execution.

The resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** using quantitative metrics and visual inspection.

---
### **Test Cases**

---
#### **CT_2D_001 — Permutative Relation (Speed Lag = 1)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** the **Speed** signal is temporally shifted by **1 sample** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to assess sensitivity to minimal temporal displacement.

---

#### **CT_2D_002 — Permutative Relation (Speed Lag = 5)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** the **Speed** signal is temporally shifted by **5 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to assess increased temporal interference.

---

#### **CT_2D_003 — Permutative Relation (Speed Lag = 10)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** the **Speed** signal is temporally shifted by **10 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to evaluate progressive temporal sensitivity.

---

#### **CT_2D_004 — Permutative Relation (Speed Lag = 25)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** the **Speed** signal is temporally shifted by **25 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to assess substantial temporal misalignment effects.

---

#### **CT_2D_005 — Permutative Relation (Speed Lag = 50)**

**GIVEN** kinematic input variables including **Latitude, Longitude, Speed, and Acceleration**  
**WHEN** the **Speed** signal is temporally shifted by **50 samples** and the system is executed  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to evaluate extreme temporal displacement and causal coherence.

---

### **Evaluation Note**

These test cases assess whether **temporal displacement of the Speed signal**, without altering its values, induces **progressive and coherent changes** in the system output, as required by the **Permutative (P)** metamorphic relation. Lack of progressive variation, erratic behavior, or execution failures are interpreted as potential violations of temporal coherence at **Metamorphic Test Level 2**.