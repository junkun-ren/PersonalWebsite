---
title: Research
nav: true
---

# Table of contents
[Current research projects](#introduction)
1. [Plankton](#paragraph1)
    1. [Model setup](#subparagraph1)
    1. [Questions to answer](#subparagraph2)
2. [Salamander](#paragraph2)


### A stoichiometry food-chain model of plankton community <a name="paragraph1"></a>
Advisor: Dr. Shaopeng Wang

<a name="subparagraph1"></a>
{% include figure.html img="plankton model illustration.png" alt="model illustration" caption="2 level food chain model with stoichiometric constrains in red<br/>This system is assumed to be carbon sufficient and closed in terms of N and P." width="85%" %}
{% include figure.html img="equations.png" alt="model equations" caption="Model equations<br/>i:N,P; j:zooplankton; k:phytoplankton" width="90%" %}

*Uptake*: there is a linear trade-off between phytoplankton's investment in N update and P uptake, indicating by p_N + p_P = 1. An increase in the relative investment in N uptake (p_N) would mean a decrease in the relative investment in P uptake meanwhile. In this model, it is also assumed that this uptake trade-off trait p_N can be an evolving trait which depends on parameter V. V is the genetic variance of this trait, V = 0 means this trait can't evolve at all. 

*Growth of phytoplankton*: it is limited by the limiting element. 

*Grazing*: besides the maximum grazing rate and predation half saturation constant, the grazing rate of zooplankton also depends on the cell element ratio difference between zooplankton and phytoplankton (i.e., nutritional quality). The probability that zooplankton will consume encountered phytoplankton follows Gaussian distribution, whose width depends on the selectivity of zooplankton. Higher selectivity gives a more narrow distribution, reducing the probability of grazing on lower quality phytoplankton. The grazing probability is maximized when consumer and producer have the same N:P ratio.

*Assimilation efficiency*: zooplankton's assimilation efficiency of ingested phytoplankton is assumed to be the lowest ratio of nutrient content of phytoplankton to nutrient content of zooplankton.

**Not only the nutrient availability is important for these processes, but also the relative amount of different elements matters**. Such constrain is shown in red in the equations. It can be seen that it is "everywhere".

{% include figure.html img="multiple zooplankton or phytoplankton illustration.png" alt="multiple zooplankton or phytoplankton illustration" caption="Model extension - more species within each trophic level" width="90%" %}

Given the single consumer-single producer model model, it is natural to wonder whether two zooplankton could coexist in this system. If two zooplankton have different demands of nutrition - one is N-demanding, the other is P-demanding, can they coexist on one species of phytoplankton? It might happen, based on theoretical prediction (`Loladze et al. 2004 - Theor. Popul. Biol.`).  Stable coexistence might occur due to a balance between food quality and quantity.

If the two zooplankton can actually coexist, will that enhance the coexistence of multiple phytoplankton as well? Because aside from phytoplankton competing for resources, the existence of zooplankton also enables the apparent competition between the phytoplankton. If there is a trade-off between two phytoplankton (resource and grazing), then one resource and one zooplankton could promote the coexistence of these two phytoplankton. Therefore, it is reasonable to predict that 2 resources and 2 zooplankton might be able to maintain the coexistence of more phytoplankton. And the coexistence of these phytoplankton can in turn support two zooplankton as well.

#### Questions to answer<a name="subparagraph2"></a>

What else to consider? Mixotroph  and


### Salamander migration <br/> <a name="paragraph2"></a>
Advisor: Dr. Dorothy Wallace

- ddd


