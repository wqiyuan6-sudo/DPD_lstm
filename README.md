# DPD-lstm-varieties
# 📘 DPD-LSTM-varieties

**Exploring the Role of LSTM Gates in Digital Predistortion (DPD)**  


## 🧠 Project Overview 

This repository investigates how each **gate component** (input, forget, output, and cell update) of the **Long Short-Term Memory (LSTM)** network affects **Digital Predistortion (DPD)** performance.

---

## 🔍 Research Background 

Digital Predistortion (DPD) is a key technique used to **linearize power amplifiers (PA)** in modern wireless transmitters.  
LSTM-based neural DPD models have shown strong ability to capture **temporal memory effects** of nonlinear PAs.

---

## ⚙️ Methodology

We design and compare several LSTM variants:

| Variant | Description |
|----------|--------------|
| **Full LSTM** | Original LSTM with all gates |
| **LSTM−F** | Removed Forget Gate |
| **LSTM−I** | Removed Input Gate |
| **LSTM−O** | Removed Output Gate |
| **Simplified Cell Update** | Modified cell state update function |

All models are trained on the same DPD dataset under identical settings to ensure fair comparison.

**Framework:** PyTorch / TensorFlow  
**Dataset:** DPA_200MHz or similar PA dataset  
**Metrics:** NMSE, ACPR, Convergence rate, N_param (parameter count)

---

## 📁 Directory Structure 

