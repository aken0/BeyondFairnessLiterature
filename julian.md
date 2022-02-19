## How ML introduces trade-offs in medicine

We have argued that there are no new fairness trade-offs at the intersection of machine learning and medicine but rather that that the preexisting ones are preserved, increased or decreased. However, the deployment of machine learning methods in the medical context does introduce new trade-offs into medicine apart from the fairness domain. So let us zoom out of this domain to see what is happening when ML and medicine are combined. 

ML tools in medicine are often discussed as a human vs. machine situation - where the ML tool outperforms the human they should and in the near future will be substituted. However, making a binary decision out of this does not seem to be the optimal solution. Different studies found that combining AI and human evaluation can achieve better results than either of the two on their own ([^1] [^2] [^3] Steiner). One of those studies also found that especially for harder cases the assisted accuracy was very high compared to the unassisted accuracy when the ML model's prediction was correct, but that it was also painfully low in cases where the ML model's prediction was incorrect [^2]. So instead of a binary decision we are left with a new situation that fits our understanding of trade-offs. How are ML and human evaluation best combined to achieve the optimal accuracy? This might heavily depend on the task at hand. For example, for skin cancer classification where the input is only a cropped image of the potential carcinoma or melanoma, the algorithms decision alone might the enough. However, for identifying diseases in a breast X-ray, a much broader task than skin cancer classification, algorithmic and human judgement might need to be combined for the optimal solution.
 maybe more AI for less experienced, less AI for more experienced? 


Often, ML tools only work for specific tools, i.e. detecting one or a couple of diseases in an X-ray. While the accuracy rate here is often high the broadness of the analysis is very limmited compared to a doctor [^3]. This could be identified as a trade-off between high accuracy with a narrow focus on the one hand and lower accuracy with a broader focus on the other.


The current way of handling medical data differs heavily from the way data is used in ML [^5]. Unfortunately, to make ML tools work properly there is a need for huge amounts of data that will be shared with the respective companies and researchers. This creates a trade-off between the classical handling of medical data and a necessary data collection.


A trade-off that is not inherent to the application of ML in medicine and health but that grows to a new importance in this field is between explainability and accuracy/performance ([^3] Limitations and challenges [^4]) . While explainability plays an important role to foster trust in ML there is probably no other field where this is as important as in medicine and health care. This can also be related to another, rather philosophical trade-off: If a person is sceptical about using ml on their diagnosis, how can we trade-off a potentially better diagnosis against respecting the persons wish with possibly risking a less accurate or even wrong diagnosis? Explainability might be a decent solution to gain the trust needed, but it might also worsen the accuracy thus actually making the mistrust in the technologie more reasonable.


The developement and deployment of ML tools in medicine and health care will and does already cost a lot of money [^5]. At the same time, the health care system in general in countries like the US is heavily underfunded. So much so that live expectancy began to decrease again in the US [^3]. Thus, there can be a trade-off identified between the financing of ML tools and the health care system in general. If the huge investments in ML tools will only benefit a small wealthier part of society, those investments are questionable if the health care systems continue to be underfunded. This is even more the case since there are not yet many ML tools ready for clinial application which makes this money an investment into the future while there persist acute issues that would need to be tackled here and now.


 Many of the trade-offs discussed can essentially be broken down to one question: How much do we benefit from the use of ML in medicine? What might be bad for us, for example could the digitalization and sharing of our health data lead to misusage by health care providers? If I know that I will most probably benefit from sharing my data on the other hand, I will be more likely to do so. This would create a very general trade-off between benefits and caveats oof ML tools in medicine and health care. ([^3] Increased Efficiencies) ([^5] Transparency)


Another trade-off exists between the way medical devices are traditionally approved for (clinical) applications and how software is usually deployed and constantly updated [^5]. While this problem might also exist with software that is already deployed in other ways in medicine and health care, ML tools take it to a new level. Here, updates might involve newly trained algorithms with a new data background which might have achieved different performance benchmarks. How should this agile updating be weighed against traditional and more accurate, but slower ways of approving tools for clinical application? In the US, the FDA already reacted by creating easier paths for approvement for this kind of software but the success of this pathway is still indeterminated.



 - In some cases, AI tools were shown to increase sensitivity but reduce specificity 
 - How much do physicians need to understand the tools they are using? ([^5] Education of an AI-literate workforce)
 - ethical question: should we predict death? ([^3] Table 3) [^5] talk about triage by ML
 - How do we study the clinical efficacy of ML tools? Is a randomized controlled trial ethical? Because with normal medical trials we do not have an alternative working treatment, we just compare it with nothing. Thus, we do not withhold something from patients. However, of ML tools (wrongfully) decide against treatment we actively withhold treatment from patients which might in extreme cases lead to their deaths. (Grote und Genin)




[^1]: [AI in healthcare and medicine](https://www.nature.com/articles/s41591-021-01614-0#Sec9)

[^2]: [Impact of a deep learning assistant on the histopathologic classification of liver cancer](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7044422/)

[^3]: [High-performance medicine: the convergence of human and artificial intelligence](https://www.nature.com/articles/s41591-018-0300-7)

[^4]: [Key challenges for delivering clinical impact with artificial intelligence](https://link.springer.com/article/10.1186/s12916-019-1426-2)

[^5]: [The practical implementation of artificial intelligence technologies in medicine](https://www.nature.com/articles/s41591-018-0307-0)

## To read

 - https://www.karger.com/Article/PDF/504785
 - https://www.jmir.org/2019/5/e13216/
 - https://www.nature.com/articles/s41746-020-0221-y
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

 