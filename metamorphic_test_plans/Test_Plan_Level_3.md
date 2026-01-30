Level 3 metamorphic tests evaluate the system under composite and dynamic driving scenarios, combining multiple input behaviors over time. This level assesses temporal coherence, regime transitions, and execution stability under realistic and critical operational conditions.

## **Scenario 3A — Steep Uphill Simulation**

**Metamorphic Relation Type:** **Composite (C)**  
_(Composite dynamic behavior under causal constraints)_

### **Description**

This scenario evaluates the system’s behavior under a **composite dynamic regime** characterized by **moderate constant speed** and **persistent positive acceleration**.

The test case simulates a **steep uphill driving condition**, in which the system is continuously subjected to increased load demand. Unlike isolated transformations applied in previous levels, this scenario combines multiple kinematic conditions into a coherent temporal pattern.

The objective is to observe whether the system produces a **stable and causally consistent output** under sustained positive acceleration, without execution interruption or erratic behavior.

---
### **Test Case**

#### **CT_3A_001 — Composite Scenario: Steep Uphill Simulation**

**GIVEN** kinematic input variables including **Latitude**, **Longitude**, **Speed**, and **Acceleration**  
**WHEN** the system is executed under a regime of **constant moderate speed** and **positive acceleration** representing a steep uphill condition  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to assess causal coherence and execution stability under sustained load.

---
### **Evaluation Note**

This test case assesses whether the system maintains **coherent output behavior** under a persistent uphill driving pattern, validating its response to continuous load increase in a composite, semantically meaningful scenario.


## **Scenario 3B — Downhill Inertia Simulation**

**Metamorphic Relation Type:** **Composite (C)**  
_(Composite dynamic behavior dominated by inertial effects)_

### **Description**

This scenario evaluates the system’s behavior under a **composite dynamic regime** characterized by **high speed** and **mild negative acceleration**, representing a **downhill driving condition dominated by inertia**.

The test case models a situation in which the vehicle progressively loses speed **without active braking**, relying primarily on inertial and gravitational effects. This configuration combines kinematic variables in a semantically coherent manner, reflecting a realistic operational pattern.

The objective is to assess whether the system maintains **causal consistency and execution stability** when subjected to gradual deceleration driven by inertia rather than abrupt control actions.

---
### **Test Case**

#### **CT_3B_001 — Composite Scenario: Downhill Inertia Simulation**

**GIVEN** kinematic input variables including **Latitude**, **Longitude**, **Speed**, and **Acceleration**  
**WHEN** the system is executed under a regime of **high speed** and **mild negative acceleration**, representing a downhill inertial condition  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to evaluate causal coherence and stability under inertia-dominated dynamics.

---
### **Evaluation Note**

This test case examines whether the system responds coherently to **gradual, inertia-driven deceleration**, ensuring that output behavior remains stable and semantically consistent in the absence of active braking forces.

---


## **Scenario 3C — Hard Braking with Fuel Cut-Off**

**Metamorphic Relation Type:** **Composite (C)**  
_(Composite critical and transient dynamic behavior)_

### **Description**

This scenario evaluates the system’s behavior during a **critical transient event** characterized by **intense negative acceleration** and **rapid reduction of speed to zero**, representing a **hard braking condition with potential fuel cut-off**.

The test case models an abrupt deceleration pattern in which vehicle motion is rapidly interrupted. Such conditions impose strong dynamic discontinuities on the input signals and are expected to induce significant changes in the system output.

The objective is to assess whether the system preserves **execution stability**, **causal coherence**, and **controlled output behavior** when subjected to sudden braking events.

---
### **Test Case**

#### **CT_3C_001 — Composite Scenario: Hard Braking (Fuel Cut-Off)**

**GIVEN** kinematic input variables including **Latitude**, **Longitude**, **Speed**, and **Acceleration**  
**WHEN** the system is executed under a regime of **abrupt deceleration**, with **high negative acceleration** and **progressive reduction of speed to zero**  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to evaluate system behavior under critical braking conditions.

---
### **Evaluation Note**

This test case examines whether the system responds coherently to **sudden, high-impact dynamic transitions**, ensuring that execution is not interrupted and that output behavior reflects the severity of the braking event in a causally consistent manner.

---
## **Scenario 3D — Constant Speed Cruise**

**Metamorphic Relation Type:** **Composite (C)**  
_(Steady-state dynamic equilibrium)_

### **Description**

This scenario evaluates the system’s behavior under a **steady-state operating condition** characterized by **constant speed** and **zero acceleration**, representing stabilized cruising typically observed during highway driving.

The test case models a dynamic equilibrium regime in which no transient events or external disturbances are present. Under such conditions, the system output is expected to exhibit **stable and consistent behavior**, reflecting the absence of acceleration-driven dynamics.

The objective is to assess whether the system maintains **output stability**, **execution continuity**, and **coherent predictions** when subjected to equilibrium input conditions.

---

### **Test Case**

#### **CT_3D_001 — Composite Scenario: Constant Speed Cruise**

**GIVEN** kinematic input variables including **Latitude**, **Longitude**, **Speed**, and **Acceleration**  
**WHEN** the system is executed with **constant speed** and **acceleration equal to zero** over the input sequence  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to evaluate output stability under steady-state conditions.

---

### **Evaluation Note**

This test case examines whether the system preserves **stable and non-oscillatory output behavior** when exposed to equilibrium dynamics, serving as a reference scenario for comparison with transient and critical events at **Metamorphic Test Level 3**.

---

## **Scenario 3E — Sudden Stop After Cruise**

**Metamorphic Relation Type:** **Composite (C)**  
_(Abrupt temporal regime transition)_

### **Description**

This scenario evaluates the system’s response to an **abrupt interruption of motion** following a stable cruising regime.

The input sequence preserves its original behavior up to sample **t = 50**, after which both **speed** and **acceleration** are forced to zero, simulating a sudden stop event. This transformation introduces a **sharp temporal discontinuity**, characterizing a rupture between steady-state operation and complete motion cessation.

The objective is to analyze whether the system produces **coherent output transitions**, maintains execution stability, and appropriately reflects the sudden change in driving dynamics.

---
### **Test Case**

#### **CT_3E_001 — Composite Scenario: Sudden Stop After Cruise (t ≥ 50)**

**GIVEN** kinematic input variables including **Latitude**, **Longitude**, **Speed**, and **Acceleration**  
**WHEN** the system is executed with original input behavior until sample **t = 50**, followed by **zero speed and zero acceleration** from that point onward  
**THEN** the resulting **Metamorphic Prediction** is compared against the **Baseline Prediction** to evaluate output coherence under abrupt temporal regime transition.

---
### **Evaluation Note**

This test case assesses the system’s ability to handle **sudden regime changes** without producing erratic behavior, execution failures, or incoherent output patterns, providing evidence of temporal consistency at **Metamorphic Test Level 3**.

