# ai-verification-spirulina-antimicrobial-tilapia
AI models (ANN &amp; ANFIS) to assess Spirulina platensis extract efficacy vs. Total Coliform &amp; S. aureus in tilapia fillets, using 600 datapoints (log CFU/g) across doses &amp; time. Includes Sugeno-type ANFIS with Gaussian MFs, LM-trained MLPs, validation metrics (DC, RMSE), and lab data from NEU's vet medicine faculty.
Spirulina Antimicrobial AI Verification
1. Overview
Tests Spirulina platensis extracts against Total Coliform and Staphylococcus aureus in tilapia fillets using AI. Quantifies dose/time-dependent bacterial reduction to validate Spirulina as a natural preservative.

2. Key Methods
Extraction:
Freeze-thaw method with 0.5g, 1g, 5g Spirulina in 100ml water (EA, EB, EC). Stored at 4°C.

Fish Samples:
100 tilapia fillets (50g each) treated with EA/EB/EC. Controls: untreated.

Microbial Analysis:
Homogenized fillets in MRD, diluted (1:10), plated on PCA. Incubation:

Total Coliform: 37°C/24h

S. aureus: 10°C/7 days
Output: log CFU/g at 1h, 24h, 48h.

3. AI Modeling
Inputs: Spirulina concentration (0.5%, 1%, 5%) + initial microbial load.

Outputs: Microbial reduction (log CFU/g).

Models:

ANN: MLP architecture, Levenberg-Marquardt training.

ANFIS: Sugeno rules + fuzzy logic (e.g., IF x=A1 AND y=B1 THEN f1=p1*x+q1*y+r1).

Validation:
75%/25% train/test split, k-fold cross-validation.
Metrics: DC, CC, RMSE, MSE (see Equations 4-7).

4. Results
Dose-dependent antimicrobial effect observed.

AI models captured non-linear interactions (e.g., pH, extraction variables).

ANFIS provided interpretable rules for industrial optimization.

5. Code & Data
Custom AI code publicly available.

Data: Experimental results from Near East University, Cyprus.

6. References
[24, 25, 26, 27, 28, 29] (See main document).

Flowcharts/equations: Embedded in original study. For full details, refer to source document.
