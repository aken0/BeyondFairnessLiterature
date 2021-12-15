# Notes

### Randomized Controlled Trials in Medical AI(2021)
- Motivates need for RCTs in Medical AI
- Shows multiple challenges/biases in RCTs as well as some mitigation

**Verdict:** probably not relevant for our topic, maybe check some of the citations

### Ensuring Fairness in ML(2018)
- Presents two case studies
- Shows different biases in mAI 
- Introduces three "Distributive Justice Options" to explain different fairness concepts (high-level overview)
- Gives recommendations on how one could incorporate fairness concerns into ML 

**Verdict:** very high level, no concrete focus on ethics, rather general fairness in mAI

### The Ethics of Machine Learning in Medical Sciences: Where Do We Stand Today?
**Source:** https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7640783/
-
-
-

**Verdict:** e

### Ethical Considerations of Using Machine Learning for Decision Support in Occupational Health: An Example Involving Periodic Workers' Health Assessments
**Source**: https://link.springer.com/content/pdf/10.1007/s10926-020-09895-x.pdf.  
**Summary**: Ethical assessment of the impact of Machine Learning Decision Support Tools in occupational health according to frameworks from medical ethics (Beauchamp and Childress) and philosophy of technology.
Ethical dilemmas arising from opposing principles.
Effects of technology on pre-existing problems.  
**Assessment**: not practical, not math. Strong on ethics. Very relevant, important discussion on several trade-offs.  
**Topics**:  
 - Philosophy of technology.
 - Beauchamp and Childress principles.
 - Case study.
 - Type: ethical deliberation.
 - Ethical issues typical of the application (problem) and of the technology (solution).
 - Conflict individual (data privacy etc.) => non-maleficence vs group => beneficence (trade-off).
 - Trade-off privacy vs predictability.
 - Trade-off non-discrimination vs predictability. 
 - Ethical dilemmas.


### Ethical limitations of algorithmic fairness solutions in health care machine learning
**Source**: https://www.thelancet.com/journals/landig/article/PIIS2589-7500(20)30065-0/fulltext.  
**Summary**: algorithmic solutions for bias are insufficient alone.
Identity could be a true predictor as well as a source of discrimination.
Fairness could reduce the efficacy of trained models, and bring to less effective treatment of patients.  
**Assessment**: Short, high-level, at most source of quotes.
**Topics**:  
 - Insufficiency of algorithmic solutions to bias.
 - Trade-off fairness-predictability.
 - Non-maleficience vs justice.
 - Protected attributes as predictors vs as sources of unequal treatment.


 ### Algorithm Fairness in AI for Medicine and Healthcare
 **Source**: https://arxiv.org/abs/2110.00603.  
 **Summary**: Honest overview of problems and solutions in applying ML to health (different applications: scans, structured data predictions, decision systems, clustering, ...). Shows how the discussion is not black-or-white, but needs to weigh fairness and efficacity. Hard to summarize, see the breadth of topics below.  
 **Assessment**: Good mix technical-ethical (mostly technical though). Some mentions of trade-offs, which are mostly secondary in the text though. Well-worth a read.  
 **Topics**: 
  - Examples of health disparities.  
  - Historical bias (p. 3); negative legacy, labeling prejudice (p. 6).  
  - Protected attributes as true predictors (p. 3, p. 16).  
  - Dataset shift (p. 4, p. 12).  
  - Trade-offs: accuracy-fairness and between different fairness measures (p. 5).  
  - Fairness technical proposals:  
    * Preprocessing: Importance Weighting (p. 6), Targeted Data Collection and Resampling (p. 8) (my note: ++ do not treat datasets as fix things).  
    * In-processing: Constraint Optimization (p. 10), Adversarial Fair Learning (p. 10).  
    * Post-processing: Calibration (p. 12). ++ discussion on individual disadvantage and accuracy trade-off: "the exclusion of individual predictions and trade-off in model accuracy highly disfavor the use of this method in criminal justice and healthcare systems." (p. 12).  
  - Challenges in AI-SaMD Deployment:  
    * Missing diversity in biomedical datasets (p. 15).  
    * Image acquisition and measurement variation (p. 18): domain/acquisition shift.  
    * Temporal dataset shift (p. 19): data generation through discriminatory processes, annotation shift (intra-observer variability, evolving clinical knowledge).  
    * Fragility of race (p. 19): unclear/different definitions, counfounders, social construct, granularity, ...  
  - Solutions:  
    * Distributed learning (against unfair dataset shift): method that insures data privacy (and compliance to rules for health data); mitigates disparate impact. But: new biases due to the participating institutions and their representation. (p. 21)  
    * Fair representation learning via disentanglement (p. 25).  
    * Model auditing using interpretability: saliency maps and perturbations (p. 27), attention-based interpretability (p. 28). => failure auditing  
  - Cool example of how subgroups can have different predictors and variable feature importance: p. 28 (EMR dataset).  
  - Distribution of roles in ensuring fairness: rules/implementation (p. 22).
  - Privacy concerns (data collections and resampling) (p. 8).  
  - Very good table with different examples of unfairness, related dataset shift, and mitigation strategies (p. 12, 13).  
  - Fairness-accuracy trade-off in disentagled representations (p. 26).  
  - Data users VS data regulators in disentagled representations (p. 26).  
