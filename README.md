Smart Grid Analytics and Optimization
This repository contains four advanced projects focused on voltage prediction and energy storage dispatch optimization for smart grids. These codes integrate machine learning models and mixed-integer optimization techniques for IEEE 123-bus and UNIFEI test systems, addressing challenges in voltage estimation, reverse power flow (RPF) utilization, and ampacity-constrained storage operation.
Repository Structure
📂 Uchenna-MGADN-EMS
├── IEEE123PCC_Regression_Used_Final_version.ipynb       # IEEE 123-Bus Voltage Prediction
├── IEEE123_RPF_Driven_Storage_MILP.ipynb                # IEEE 123-Bus Storage Dispatch Optimization
├── UNIFEIPCC_Regression_Used_Final_version.ipynb        # UNIFEI Voltage Prediction
├── UNIFEI_RPF_Driven_Storage_EV_Optimal_Dispatch.ipyn   # UNIFEI Storage Dispatch Optimization
Project Summaries
1. IEEE 123-Bus Voltage Prediction (IEEE123PCC_Regression_Used_Final_version.ipynb)
Predicts three-phase voltages using Neural Networks (PyTorch), Linear Regression, and XGBoost. Includes advanced feature engineering (irradiance, power, cyclic time encodings), blocked cross-validation, and hyperparameter tuning with Optuna. Outputs include deployment pipeline and high-resolution plots comparing actual vs predicted voltages.
2. IEEE 123-Bus Storage Dispatch Optimization (IEEE123_RPF_Driven_Storage_MILP.ipynb)
MILP-based optimization using Pyomo and Gurobi for energy storage scheduling. Objective: maximize RPF-based charging and cost-efficient discharging while enforcing ampacity limits and operational policies. Outputs include optimal dispatch schedule, KPI dashboard, and plots for energy state, charging/discharging power, and net PCC power.
3. UNIFEI Voltage Prediction (UNIFEIPCC_Regression_Used_Final_version.ipynb)
Predicts PCC voltages using Neural Networks, Linear Regression, and XGBoost. Features hyperparameter optimization via Optuna and randomized search for XGBoost. Includes deployment-ready pipeline and comparative plots for actual vs predicted voltages in per-unit format.
4. UNIFEI Storage Dispatch Optimization (UNIFEI_RPF_Driven_Storage_EV_Optimal_Dispatch.ipyn)
MILP optimization for storage and EV charging under ampacity constraints. Implements dynamic Pmax calculation based on voltage and current limits, policy enforcement for RPF charging and high-price discharging. Outputs include optimal dispatch schedule, KPI dashboard, and presentation-ready plots.
Why These Projects Matter
These codes demonstrate how data-driven models and optimization techniques can enhance grid reliability, DER integration, and economic dispatch. They provide scalable solutions for voltage prediction, storage scheduling, and compliance with ampacity and operational constraints for safe grid operation.
Getting Started
Prerequisites:
- Python 3.8+
- Libraries: PyTorch, Pyomo, Gurobi, Optuna, XGBoost, scikit-learn, pandas, matplotlib

