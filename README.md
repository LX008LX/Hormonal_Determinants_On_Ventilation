# Hormonal Determinants On Ventilation
## Biomedical Data Analytics & Mixed-Effects Modeling of Ventilation Under Hypoxia

This project analyzes how hormonal status, oxygen condition, and exercise intensity affect women’s ventilation during exercise, using a full R-based statistical modeling workflow. The dataset includes both premenopausal and postmenopausal participants measured under hypoxia and normoxia, with complex individual variability and partially missing hormone data.

🔬 Project Overview

Using the dataset provided by a biomedical research client, we implemented a hierarchical mixed-effects modeling pipeline to quantify how ventilation changes across:
- Oxygen condition (hypoxia vs. normoxia)
- Menstrual cycle phases (younger women)
- Hormone replacement therapy (older women)
- Exercise intensity (% peak power)
- Participant-level random effects
  
We conducted full model selection (VIF filtering, backward elimination), imputation for missing hormone measures, and validation across cohorts.

📊 Key Findings
- Hypoxia strongly increases ventilation across all participants.
- HRT significantly attenuates ventilatory response under hypoxic stress in older women (negative hypoxia × HRT interaction).
- Fitness level (VO₂max) positively predicts ventilation.
- No statistically significant effect of progesterone or estradiol in younger participants.
- Substantial individual heterogeneity was captured through random intercepts in the mixed-effects models.

🧰 Tech Stack
- R, tidyverse, lme4, ggplot2, broom.mixed
- Model diagnostics & multicollinearity checks (VIF)
- Data cleaning, imputation, transformation
- Statistical visualization and interpretation
- Reproducible analysis scripts & client-ready reporting

🧪 Methods
- Uniform imputation for sparse hormone variables
- Hierarchical linear mixed-effects models
- Interaction modeling (e.g., hypoxia × HRT)
- Model comparison via AIC, p-values, and effect sizes
- Visual analysis (interaction plots, predicted ventilation curves)
- Cohort validation through combined and stratified models

📄 Deliverables
- Full client-facing statistical report summarizing findings
- Scientific poster visualizing model outputs and interactions
- Reproducible R scripts for cleaning, modeling, and diagnostics

🚀 Impact

This project provides a robust, reproducible modeling pipeline for studying ventilation responses in women’s exercise physiology. Findings highlight the nuanced role of HRT in respiratory adaptation to hypoxia and support more rigorous experimental design for future biomedical research.
