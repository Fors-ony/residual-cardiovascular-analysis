RESIDUAL CARDIOVASCULAR RISK BEYOND CONVENTIONAL LIPID PROFILE(LDL-C)
A data analysis project that asks a simple question: Among people whose LDL-C is already low how many still show other lipid abnormalities that carry cardiovascular risk

#Important notice: The dataset is synthetic. This project demostrate a method. It does not provide clinical evidence and the result must not be used for any clinical decision.
# What this project does
1. Loads and checks a 9000 row lipid and risk factor dataset
2. Converts triglycerides and HDL-C from mg/dl to mmol/L
3. The main analysis filters to people with LDL-C < 100mg/dl and measures how many still have
 • high triglycerides (≥ 150 mg/dL)
 • raised remnant cholesterol (total cholesterol − LDL-C − HDL-C (>30mg/dl)
 • raised non-HDL-C (≥ 130 mg/dL)
4. The secondary analysis calculates the Atherogenic Index of Plasma, AIP = log10(TG / HDL-C), groups people as low (< 0.11), intermediate (0.11–0.21) or high (> 0.21) risk, and compares lipids and heart disease prevalence across groups

# Results
• 4052 people had Ldl-c < 100mg/dl. of these 59.9% had at least one abnormal marker, Triglyceride -49.4%, Remnant cholesterol -49.9% Non HDL-15.8%
• AIP mean 0.006(SD 0.21), 57.0% low, 20.3% intermediate and 22.7% high risk
•LDL-C barely changed across AIP groups (101.4 to 103.9 to 107.5 mg/dL), while HDL-C fell (60.6 to 43.8 mg/dL), triglycerides rose (122.5 to 205.6 mg/dL) and heart disease prevalence rose (23.3% to 32.3% to 46.2%).

# Dataset
Heart Disease Risk 2026 by uditjain13, Kaggle, licence CC0 (public domain). It is entirely synthetic and generated with NumPy for practice.
# How to run
pip install pandas numpy matplotlib jupyter 
jupyter notebook residualrisk_analysis.ipynb
# Tools
Python, Pandas, Numpy, Matoplotlib, Jupyter Notebook

