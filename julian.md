## How ML introduces trade-offs in medicine

We have argued that there are no new fairness trade-offs at the intersection of machine learning and medicine but rather that that the preexisting ones are preserved, increased or decreased. However, the deployment of machine learning methods in the medical context does introduce new trade-offs into medicine apart from the fairness domain. So let us zoom out of this domain to see what is happening when ML and medicine are combined. 


At least one study found that combining AI and human evaluation can achieve better results than either of the two on their own [^2]. The same study also found that especially for harder cases the assisted accuracy was very high compared to the unassisted accuracy when the ML model's prediction was correct, but that it was also painfully low in casse where the ML model's prediction was incorrect.


 - Often: human vs AI, although there might be ways around this [^1]
 - Question that remains: How are the two best combined? [^1]
 - In some cases, AI tools were shown to increase sensitivity but reduce specificity 
 - maybe more AI for less experienced, less AI for more experienced? 
 - A rather philosophical trade-off: If a person is sceptical about using ml on their diagnosis, how can we trade-off a potentially better diagnosis against respecting the persons wish with possibly risking a less accurate or even wrong diagnosis?



[^1]: [AI in healthcare and medicine](https://www.nature.com/articles/s41591-021-01614-0#Sec9)

[^2]: [Impact of a deep learning assistant on the histopathologic classification of liver cancer](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7044422/)
