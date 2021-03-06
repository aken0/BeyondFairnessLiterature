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


### The ethics of AI in health care: A mapping review
**Source**: https://www.sciencedirect.com/science/article/abs/pii/S0277953620303919.  
**Summary**: Review of existing literature on the ethics of AI in health care.
Divides ethical issues in epistemic, normative (fairness...) and traceability issues.
Distinguishes levels of abstraction: individual, interpersonal, group, institutional, and societal or sectoral.  
![summary_1](figures/ethics_ai_healthcare_table_1.png)
![summary_2](figures/ethics_ai_healthcare_table_1.png)
![summary_3](figures/ethics_ai_healthcare_table_1.png)  
**Assessment**: Non-technical, socio-philosophical.
Of particular interest to us is 3.2 Normative concerns.
The first paragraph of page 5 is definitely something we should use, as a seed for sources as well!
Very interesting to deep down into the "individual's integrity of self harm => maleficience" and find counter-arguments.
Interesting distinction of levels of abstraction, which can link to a discussion of trade-offs individual-group.
But: not much is said about trade-offs (see: points of critique).
In general, this is a big problem I have with the paper: they do not seem (to me) to recognize that many of the problems they point to are inherent to the medical problem and not to the algorithmic solutions.
This makes for a good starting point for our paper: showing how trade-offs and ethical problems are mostly inherent to the application domain, and not to algorithmic solutions.
ML just makes them visible and unavoidable instead of implicitly shifting them onto practitioners.
I think Bob had a similar point in the lecture about technology.  
**Topics**:  
 - AI for clinician support (cooperation) and not replacement (p. 2).  
 - Proactivity: make sure to avoid errors to avoid early social rejection (p. 2).  
 - Biomedical ethical principles well-developed (p. 2).  
 - Challenge: current research limited to single fields instead of interaction, focused on individual level impacts, does not consider variability of ethical concerns depending on algo development stage (p. 2).  
 - Only recommendations not necessarily a solution: clinicians might rely too heavily/behave uncritically => overreliance, deskilling of practicioners (p. 4).  
 - Epistemic level:  
  * Advantages of AI: evidence-based decisions, most informed decision (more data), can operate at scale (p. 3).  
  * Doubts on objectivity: meaninglesness of patterns, overfitting, lack of reproducibility, untranslatability, scientific rigor, safety, results heavily value-laden (p. 3).  
  * Individual LoA (level of abstraction): risk of misdiagnosis (malfunctionment, HCP relying too heavily/uncritically on recommendation) (p. 4).  
  * Group LoA: misdiagnosis repeated => scale of solution = scale of problems (p. 4).  
  * Interpersonal LoA: trust and empathy, de-humanisation, impersonalization, paternalism which could also lead to poorer outcomes due to disconnect between pure medical evidence and actual behavior change (p. 4).  
  * Institutional, sectoral, societal LoAs: increasing use of AI-health algos in public health decisions: flawed assumptions=>poor-quality evidence; data sharing private-public; quality of data transformation process (p. 4).  
- Normative level:
  * "it would be ethically remiss to ignore these opportunities" (p. 4), but those opportunitites "are not created by AI-Health technologies per se but by their ability to fundamentally change the intrinsic nature of the ways in which healthcare is delivered by coupling, re-coupling and de-coupling different parts of the system.". This relates to the lecture on AI as a technology/tool.  
  * AI-health couples patients and their data (patients ARE their data), re-couples research and practice, de-couples presence of HCP (healthcare providers) and location of the patient (p. 4).  
  * Individual LoA: (opaque) data sharing=>privacy, **less involvement in decisions undermines individual autonomy** (need: understanding of data AND methods: ehealth literacy difficult and black-box algos). Damage to individuals's integrity of self because their confidence to refuse treatment is attacked; this can be seen as a harm, **contrasting with non-maleficience** (p. 5). On the clinician's side, risk of being left on the side/being unsure about exerting their own agency, but uncertainty of the situations can only be resolved by physicians.  
  * Group LoA: AI might only be able to recognize illnesses/... that have fairly set protocols, and only fit groups for which many examples are available. This might exacerbate existing inequalities, benefitting those groups that generate enough data. Algorithms might "ignore outliers", providing a basis for discrimination. Instituitions should decide what can be delegated to AI, and base their decisions on whether healthcare is "seen as a means of promoting social justice", on "which values should be embedded in algorithmic decision-making services", and "what sort of population-level behavioural change the health system should be able to aim for".  
  * Sectoral LoA: "risk of privately held AI-health solutions, trained on datasets that have been generated about the public by public actors but then (lawfully) shared with private companies" could give them a lead advantage and make the public sector dependent on those initially chosen companies.  
  * Societal LoA: society must decide values of care before applying AI-health (is human interaction important?). How should factors (AI prediction vs clinician's personal judgement) be weighted? Direct involvement of the public in designing AI-health (public opinion data) may be necessary/help.  
 - Traceability level:  
  * Healthcare systems rely on "interactions between human, artificial, and hybrid agents [...] making it increasingly challenging to identify interaction-emerging risks and allocate liability, raising ethical concerns with regards to moral responsibility". (p. 6)  
  * AI-health solutions: data collected, transformed, analyzed, ... decision-making a black box, entire chain comples => no clear causal chain of given outcome => inaccessible and opaque ecosystem.  
  * Example monitoring system:
    - Individual LoA: Advice from AI device might not be followed for a lot of reasons (and might have been wrong), but if something happens and the individual did not follow the advice, could lead to victim blaming. This might all "shift the ethical burden of 'living well' squarely onto newly accountable individuals". (p. 6).  
    - Group LoA: underperformance on some groups => advice less followed => group seen as "more morally irresponsible about their healthcare".  
    - Interpersonal/institutional/sectoral LoAs: responsibility=>liability (liability issue must be resolved before adoption). HCP providing advice based on algo => medical malpractice when it goes wrong? Common thesis: explainability is the answer => once algo explainable, it might even be medical malpractice to not rely on the algo's output.  
  * Society will decide what is acceptable, but who is society? Who has a say, how much do they count?  
 - Distinguish: type of concern, LoA, development stage of algorithm (p. 8).  
 - Need balance between protecting individuals from harm and support innovation and its benefits (p. 8). "'there cannot be exceptionalism for AI in medicine,' expecially not when there is potentially so much to gain".  
**Points of critique**:  
In page 5, while discussing fairness and better accuracy to a group, the authors forget to mention trade-offs.
Should we discard available information about a group just to have predictions that are "as bad as those for other groups"?
What is the difference with clinicians: do they not also learn from examples, and implicitly learn better for a group/overfit on it?
The comparison AI-humans seems missing in this point.
Furthermore, it seems to imply that AI algorithms can only focus on macro accuracy.  
P. 6 monitoring systems example, individual LoA: how is this different from medical advice given by humans?


### Addressing Fairness, Bias, and Appropriate Use of Artificial Intelligence and Machine Learning in Global Health
**Source**: https://www.frontiersin.org/articles/10.3389/frai.2020.561802/full  
**Summary**:  
As the title says: fairness, bias, and appropriate use of AI in global health (particularly: low- and middle-income countries).
After a theoretical discussion, they present a case study in which they outline how to assess fairness and bias at different stages of the (development) pipeline.  
![Analysis_of_bias_in_the_development_pipeline](figures/bias_pipeline.jpg)  
**Assessment**: Nice and nuanced.
Point out how many ethical choices are subjective and somewhat arbitrary.
Mention trade-offs, many overlapping points with Bob's lectures.
Some presence of math ++.  
Interesting evaluations that show how many problems are not proper to the technology but to the problem (see Bob's lectures).  
**Topics**:  
 - Examples of applications of ML to medicine and global health (p. 2).  
 - Potential harms greater in LMIC (low- and middle-income countries): marginalized populations and greater discrimination, lacking legal and regulatory framework, current health disparities that could be exacerbated (p. 2).  
 - Ethics come into play when deciding on the operating point of the algorithm, which decides on a trade-off false positives vs false negatives that is often debated in medicine => not ML-specific (p. 3).  
 - Group differences in medicine caused by biological differences (/genetic), cultural/behavioral differences, environmental factors, confounding variables; unbalanced datasets (political weight/demographic weight) (p. 3).  
 - 3 criteria of evaluation of ML systems: appropriateness, bias, fairness.  
  * Appropriateness: assessed before deployment, = ML matches the specific context and population? (see Williamson's last choice, "data" lecture). Importance of the context (the problem is not the algorithm, see Williamson's "technology" lecture) => need for domain knowledge. Interpretability is often desired by doctors. Unbalanced datasets are a problem, and one should adapt to the specific population. "the proper balance between sensitivity (true positive rate) and specificity (true negative rate) is ultimately a subjective decision that depends on the application objectives and relies on the ethical principles being adopted." (p. 5). Solutions to imbalanced datasets: resampling, ensemble methods, cost functions and hyperparameter tuning, combinations.  
  * Bias: data bias is caused by flaws in human design. != Algorithmic bias is independent of ethics (bias is judged unfair from legal or ethical point of view) (p. 6).  
    - Causes of bias: implicit (e.g. unforeseen correlations) vs explicit causes (e.g. sampling bias, batch effect in measurements).  
    - Mitigation of bias: data collection and sampling process, data processing, feature extraction, regularization techniques, cost functions, post-processing => test for bias at all stages!  
    - Bias may still be tolerated in some contexts, but must be documented (p. 7).  
  * Fairness: Individual or group level.  
    - Consistency definition: similar features => similar treatment (p. 7). Practice: need to work at the group level (laws and algorithms). But: in medicine, those attributes might be important features (predictors).  
    - Fairness is quantified in ML when determining the optimum operating point (ROC curve) (p. 7).  
    - Definitions of fairness, contrasts (nothing new here); "In the case of medical diagnostic tests, the equality of odds criterion is often chosen [...]" (p. 8); when the criterion decreases performance much, consider using different models.  
    - Transparency: the developers of ML systems for medicine may need to disclose the conditions of validity of a model (p. 8).  
 - Interesting case study. Lessons learned:  
  * If bias in the results persists when using balanced training data, the problem is not sampling bias in the training data (p. 11).  
  * Examine feature differences between the groups of interest (eg smokers/non smokers) and see how they correlate to the target variable (and if the result is expected). Then possibly stratify based on that feature (pp. 12-13).  
  * Finally, adjust the baseline probability (prior) based on the target population (p. 14).  
 - Conclusions: LMICs particularly problematic for absence of legal framework and existing disparities; medical care and health tracking applications offer opportunities and risks.  
 - Recommendations (general: medical problems often include hidden variables and correlations; domain expertise is necessary):  
  * Question appropriate use (ML requires precise questions)  
  * Maintain transparency for critical decisions  
  * Enforce transparency in data and algorithms  
  * Address and respect bias at each level of the computation (sampling bias, implicit cultural bias, true systematic bias inherent in biological processes)  
  * Agree on a fairness metric ("While individual fairness is a good ideal, most laws are written with respect to group fairness [...] it should be recognized that trade-offs and compromises will often need to be made, to reconcile how the benefit and the risk will be shared across all groups." (p. 16))  


### On the apparent conflict between individual and group fairness  
**Source**: https://arxiv.org/pdf/1912.06883.pdf  
**Summary**: Individual and group fairness measures are not necessarily based on different ethical/normative principles.
  Both of them are compatible with egalitarianism and consistency, and not with individual justice.
  There is thus no intrinsic trade-off between individual and group fairness.
  Plus, we can use both kinds of measures to implement different normative principles (in a way, they are equivalent).
  The real difference in problems, where a trade-off is needed, is in worldviews: what is the cause of output differences for different groups?
  This is a consequence of the assumptions we make about the world/our data.  
**Assessment**: For sure a useful source for the individual vs group trade-off discussion (more on the ethical side).
  Although the author's thesis is that such a trade-off is not needed, in my view he simply shifts the discussion (better reterms the problem).
  The trade-off becomes an assumption about how much of the differences between two groups is caused by structural injustice and how much by individual differences.  
  Not related to medicine/health, but it might be interesting to see how the idea translate.  
**Topics**:  
 - Description of the conflict individual/group fairness in the context of fair ML: group fairness (e.g. in statistical parity) harms consistency. Lack of principled discussions in fair-ML.  
 - The real cause of the conflict in practice are constrasting (unstated) assumptions about the world/context.  
 - Description and problems of individual/group fairness measures in fair-ML (ch. 2.1), balance and trade-off (ch. 2.1.3).  
 - Principled discussion: the real underlying principles are consistency (often related to individual fairness) and egalitarianism (oftern related to group fairness).
 Although they have natural correlations to group/individual fairness, they are in reality compatible to both (and both are compatible with each other).  
 - Individual justice cannot be followed by any automated system (requires "case-by-case" decisions), and is incompatible with both fairness measures (individual fairness still equates and individual with its set of features).  
 - In practice, the problem lies in the assumptions about the nature of differences: luck/systemic injustice OR individual choice.  
 - It is difficult to decide on the assumptions; hence, one solution always remains not to use ML in the first place (5.3.1) (see Bob's lecture). Assumptions can't be avoided.  
 - Conclusion: maybe we should concentrate more on the data-generating process (underlying structures).  
**Comments**:  
 - It is not at all surprising that the problem comes down to be a problem of assumptions.
 - We know that ML models are based on assumptions (inductive bias), and cannot learn without them.  
 - On consitency: arguably, most ML models (among all, regression) respect consistency because they learn continuous functions (and even more, if L2-regularization is applied) IF WE EXCLUDE CATEGORICAL VARIABLES.  
 - Critique the sentence "the individual fairness distance metric could represent a rough consensus about how disadvantaged certain groups are in a given context" (5.1): nice and all, but how will this measure be determined in practice? I argue, based on statistics (statistical parity); so in the end, it comes down to the same problem: how to weigh the different causes of differences when we have no quantitative idea?  
 - Application of the reasoning line to medicine appears more complicated: should we be concerned about egalitarianism at all in medical settings, and not obtaining the best results possible? If non-maleficience outweighs beneficience as a principle, then is it justify to insert UNVERIFIED ASSUMPTIONS about the nature of bias into a model, knowing that it will decrease its predictive power?  
 - In the end, when we make assumptions about the nature of bias, we end up (even on an ideal/normative level) choosing a trade-off when applying a "data correction". Reasoning with uncertainty, we might e.g. decide to correct less for systemic bias because we find it more problematic to correct too much rather than too little (we prefer systemic bias over individual unfairness).  
 - Since we don't know the nature of the errors in the data, the only acceptable solutions seems to be not using the data.  

