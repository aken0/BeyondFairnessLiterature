## Structure

### Introduction

### Tradeoffs in general (Thomas?)

From Lecture 1:

- The loss function encodes what we care about. What do we want our model to be good at? How can we express this mathematically?
- Iverson brackets [[p]] = 1 if p is true, = 0 if p is false

### Tradeoffs in machine learning

### tradeoffs in Medicine (arthur hat angefangen)

### tradeoffs at the intersection of machine learning and medicine (arthur & Julian)

##### fairness tradeoffs are not new to medicine (arthur)

##### but other (ethical?) tradeoffs are new (julian)

### conclusion


## General (Introduction?)

Machine Learning (ML) in health care and medicine has grown to be one of the most discussed, but also most promising applications of the ever-growing technology of ML. In recent years, more and more research has shown ML to be an effective way of supporting health care practitioners in a great diversity of ways [^1] [^3]. However, there is also growing concern about the implications the deployment of ML has for the future of health care and medicine.

While there are ongoing public discussions about ML replacing humans as workers in many different ways [citation needed], many scholars have made clear that ML and AI tools will not replace clinicians in the near future but rather be integrated as support systems, for example as clinical decision support systems (CDSS) [^a1].

CDSS have been used since the 1980s with growing success [^7]. Only in recent years, the involvement of Machine Learning in those systems has led to a new regulatory situation. Still, their deployment and success can tell us a lot about the way to go with ML tools. For example, although closed loop systems, i.e., systems were every step of the process from diganosis to drug intake is computerized and monitored, do already exist they are not commonly used, partly due to costs but certainly also due to the involved surveillance environment for patients [^7].




## Arthur

We do not, however, argue that ML does not introduce any new ethical problems, but that they are not fairness-related.
For example, ML systems applied at a large scale unify decisions, exponentially increasing the impact of failures.
Less federated decisions make for less error-robust systems, and unified treatment and strategy gives fewer indications about what works well, potentially reducing the possibilities for learning from single experiences.
Additionally, automated decision systems distribute the responsibility for the decisions the system takes, making it very difficult to attribute responsibility for potential misjudgments [^a1].
If the decisions are not taken automatically, the practitioner might still rely too much on them and avoid a right call that would contradict the suggestion of the ML system [^a1]  (automation bias, [^a2]).
Additionally, they might pay less attention to the decisions that are assisted by technology.
The complex models of ML and the large amount of features used help make more personalized decisions for the individual, but decrease their understandability [^a2].
The lack of explainability of the decisions taken by automated systems might additionally contrast with the biomedical principle of the respect of autonomy, since it reduces the patient's possibility to exert informed consent [^a3].
Finally, the trust of the public in the decisions taken by automated decision systems may be low, making their large-scale use politically difficult [^a1].



## How ML introduces trade-offs in medicine

We have argued that there are no new fairness trade-offs at the intersection of machine learning and medicine but rather that the preexisting ones are preserved, increased or possibly decreased. However, the deployment of machine learning methods in the medical context could introduce new trade-offs into medicine apart from the fairness domain. So let us zoom out of this domain to see what is happening when ML and medicine are combined.


A trade-off that is not inherent to the application of ML in medicine and health but that grows to a new importance in this field is between explainability and accuracy/performance ([^3] Limitations and challenges [^4]) . While explainability plays an important role to foster trust in ML in general there is probably no other field where this is as important as in medicine and health care. Unfortunately, explainable ML approaches have yet to reach the same level of performance as other ML systems. Thus, the need for explanations results in a trade-off between how good the explanations are and how good the system performs in terms of accuracy.
The issue of trust in the technology can also be related to another, rather philosophical trade-off: If a person is sceptical about using ml on their diagnosis, how can we trade-off a potentially better diagnosis against respecting the persons wish with possibly risking a less accurate or even wrong diagnosis? Explainability might be a decent solution to gain the trust needed, but it might also worsen the accuracy thus actually making the mistrust in the technology more reasonable.
If it is impossible to reach a conclusion, for example because there is not enough data, ML tools should be transparent about that and indicate that they cannot make a decision rather than making a bad informed decision [^6]


ML tools in medicine are often discussed as a human vs. machine situation - where the machine outperforms the human they should and in the near future will be substituted. However, making a binary decision out of this does not seem to be the optimal solution. Different studies found that combining AI and human evaluation can achieve better results than either of the two on their own ([^1] [^2] [^3] Steiner). One of those studies also found that especially for harder cases the assisted accuracy was very high compared to the unassisted accuracy when the ML model's prediction was correct, but that it was also painfully low in cases where the ML model's prediction was incorrect [^2]. So instead of a binary decision we are left with a new situation that fits our understanding of trade-offs. How are ML and human evaluation best combined to achieve the optimal accuracy? This might heavily depend on the task at hand. For example, for skin cancer classification where the input is only a cropped image of the potential carcinoma or melanoma, the algorithms decision alone might the enough. However, for identifying diseases in a breast X-ray, a much broader task than skin cancer classification, algorithmic and human judgement might need to be combined for the optimal solution. There is also evidence that AI might especially improve the performance of less experienced practioners like those who are still in training while those who are already experienced would not profit as much [^1]. This brings another level into the trade-off because experienced practioners who already perform on a similar level as the AI the necessitation to use the technology might even be hindered by another step in their workflow. In fact, for CDSS without ML components it was already observed that more experienced doctors ignore its assistance more often without performing less good [^7].

the more ML tool and physician interact, the harder it gets to identify responsibility (partly [^6])
How much do physicians need to understand the tools they are using? ([^5] Education of an AI-literate workforce)

ML tools are said to be able to increase efficiency in hospitals and prevent unnecessary hospital visits, thus reducing pressure on care workers and doctors, which is certainly a good thing [^6]. However, it will be important to take a holistic approach towards health care in the future. ML tools are too often seen as the holy grail to solve problems when in fact they are just tools that will not tackle structural problems without using them to do so. For example, in current health care systems reduced workload of care workers has the potential to lead to a reduction in the workforce because it is a way to save money. However, this would then not lead to an actual improvement for patients but only to a potential financial reward. This can be seen as a trade-off between monetary outcomes and spendings on the one  and the patients experience and care on the other hand. While this is an issue that is already existing, ML tools bring another perspective to it since they have the potential to increase as well as heavily decrease the patients experience in hospitals.


Some scholars argue that while a mistake by a human practioner only affects a small amount of people (often only one person), a mistake by an algorithm that is deployed on many hospitals will happen more often and thus affect more people [^a1]. This could be seen as a trade-off between the scale of deployment of a technology and the severity of mistakes. However, this argument can also be seen as flawed since although one practioner might not repeat a certain mistake, other practioners not involved in this situation might well do. Thus, the only argumentation here could be that the errors are not as systematically spread as with ML tools, although even that might be an overstatement.


Another Trade-off can be seen between empathy in human practitioners and a more standardized way of tackling tasks in ML tools [^a1]. What do we understand as good health care, only the right diagnosis or psychological wellbeing during treatment, etc. as well?
ethical question: should we predict death? ([^3] Table 3) [^5] talk about triage by ML

Often, ML tools only work for specific tasks, i.e. detecting one or a couple of diseases in an X-ray. While the accuracy rate here is often high the broadness of the analysis is very limited compared to a doctor [^3]. This could be identified as a trade-off between high accuracy with a narrow focus on the one hand and lower accuracy with a broader focus on the other.


The current way of handling medical data differs heavily from the way data is used in ML [^5]. Unfortunately, to make ML tools work properly there is a need for huge amounts of data that will be shared with the respective companies and researchers. This creates a trade-off between the classical handling of medical data and a necessary data collection.

Health care systems around the world are more or less privatized, depending on the country. However, in the case of ML tools a lot of research and development is driven by big companies like Alphabet or IBM [^a1]. This makes sense since those companies are driving ML research in general but it poses the question whether we want to give such an important issue completely out of public and into private hands. While the privatization of health care was already posing problems before ML tools and they are in fact seen as a solution for the existing problems [^a1] [^3], the questioning of privacy and trust is increased as well. Thus, this can be seen as a trade-off between the speed of development - arguably, big tech companies will be fast in bringing ML tools to the market - and privacy and trust issues.


The development and deployment of ML tools in medicine and health care will and does already cost a lot of money [^5]. At the same time, the health care system in general in countries like the US is heavily underfunded. So much so that recently, life expectancy began to decrease again in the US [^3]. Thus, there can be a trade-off identified between the financing of ML tools and the health care system in general. If the huge investments in ML tools will only benefit a small wealthier part of society, those investments are questionable if the health care systems continue to be underfunded. This is even more the case since there are not yet many ML tools ready for clinical application which makes this money an investment into the future while there persist acute issues that would need to be tackled here and now.

WTF?  The savings would come from a combination of deployments: lower medical costs and reduced losses from low productivity and sick day ([^6] page 148)

Another trade-off exists between the way medical devices are traditionally approved for (clinical) applications and how software is usually deployed and constantly updated [^5]. While this problem might also exist with software that is already deployed in other ways in medicine and health care, ML tools take it to a new level. Here, updates might involve newly trained algorithms with a new data background which might have achieved different performance benchmarks. How should this agile updating be weighed against traditional and more accurate, but slower ways of approving tools for clinical application? In the US, the FDA already reacted by creating easier paths for approbation for this kind of software but the success of this pathway is still indeterminated.
Today, regulation processes are often such that the model is locked in place before deployment. This makes it easier to regulate them but misses out on their potential to learn and increase functionality on the fly. [^ted1]
How do we study the clinical efficacy of ML tools? Is a randomized controlled trial ethical? Because with normal medical trials we do not have an alternative working treatment, we just compare it with nothing. Thus, we do not withhold something from patients. However, of ML tools (wrongfully) decide against treatment we actively withhold treatment from patients which might in extreme cases lead to their deaths. (Grote und Genin)

Many of the trade-offs discussed can essentially be broken down to one question: How much do we benefit from the use of ML in medicine? What might be bad for us, for example could the digitalization and sharing of our health data lead to misusage by health care providers? If I know that I will most probably benefit from sharing my data on the other hand, I will be more likely to do so. This would create a very general trade-off between benefits and caveats of ML tools in medicine and health care. ([^3] Increased Efficiencies) ([^5] Transparency)
Can digital health care be for everybody? what about people who do not have digital devices or don't want to use them? [^ted2]

But this also leads to the question whether these trade-offs are actually new or - as discussed for fairness trade-offs above - if they are just new editions of trade-offs humanity has seen before in either ML, medicine and health care or technology in general.



[^1]: [AI in healthcare and medicine](https://www.nature.com/articles/s41591-021-01614-0#Sec9)

[^2]: [Impact of a deep learning assistant on the histopathologic classification of liver cancer](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7044422/)

[^3]: [High-performance medicine: the convergence of human and artificial intelligence](https://www.nature.com/articles/s41591-018-0300-7)

[^4]: [Key challenges for delivering clinical impact with artificial intelligence](https://link.springer.com/article/10.1186/s12916-019-1426-2)

[^5]: [The practical implementation of artificial intelligence technologies in medicine](https://www.nature.com/articles/s41591-018-0307-0)

[^6]: [Artificial Intelligence: Power for Civilisation – and for Better Healthcare](https://www.karger.com/Article/PDF/504785)

[^7]: [An overview of clinical decision support systems: benefits, risks, and strategies for success](https://www.nature.com/articles/s41746-020-0221-y)

[^8]: The AI of ethics


[^a1]: [The ethics of AI in health care: A mapping review](https://drive.google.com/file/d/1Cwpwwp-e6oBu-V_7PoATDNSXsWyjKvjf/view)
[^a2]: [Ensuring Fairness in Machine Learning to Advance Health Equity](https://www.acpjournals.org/doi/pdf/10.7326/M18-1990)
[^a3]: [Ethical Considerations of Using Machine Learning for Decision Support in Occupational Health: An Example Involving Periodic Workers’ Health Assessments](https://link.springer.com/article/10.1007/s10926-020-09895-x)


[^ted1]: [Artificial intelligence in healthcare: opportunities and challenges | Navid Toosi Saidy | TEDxQUT](https://www.youtube.com/watch?v=uvqDTbusdUU)

[^ted2]: [Artificial Intelligence in Healthcare - The Need for Ethics | Varoon Mathur | TEDxUBC](https://www.youtube.com/watch?v=4oPpSFp87iE)

[^ted3]: [Artificial Intelligence Meets Mental Health Therapy | Andy Blackwell | TEDxNatick](https://www.youtube.com/watch?v=ZkTvw3usMw4)


## To read

 - https://www.jmir.org/2019/5/e13216/
 - https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7437567/
 - https://link.springer.com/article/10.1186/s12911-020-01191-1
 - https://www.liebertpub.com/doi/pdfplus/10.1089/omi.2019.0038
 - https://i-jmr.org/2019/2/e12100
 - https://www.frontiersin.org/articles/10.3389/fdgth.2020.00006/full
 - Steiner, D. F., et al. Impact of Deep Learning Assistance on the Histopathologic Review of Lymph Nodes for Metastatic Breast Cancer.
 - Holzinger A, Biemann C, Pattichis CS. What do we need to build explainable AI systems for the medical domain?
 - Sayres R, Taly A, Rahimy E, Blumer K, Coz D, Hammel N, et al. Using a deep learning algorithm and integrated gradients explanation to assist grading for diabetic retinopathy.
 - Char, D. S., Shah, N. H. & Magnus, D. Implementing machine learning in health care—addressing ethical challenges
 - Jiang, F. et al. Artificial intelligence in healthcare: past, present and future

## read, but not cited

 - https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0212356
 - Artificial Intelligence for Global Health: Learning from a Decade of Digital Transformation in Health Care https://arxiv.org/pdf/2005.12378.pdf
 -
