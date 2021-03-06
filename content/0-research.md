---
title: Research
nav: true
---

##### Current research projects <a name="top">
1. [An eco-evolutionary stoichiometry food-web model of the plankton community](#paragraph1)
    1. [Model setup](#subparagraph1)
    2. [Model extension](#subparagraph2)
    3. [Questions to answer](#subparagraph3)
    4. [Example results](#subparagraph4)
2. [Modeling tiger salamander's migration and phenotypic plasticity](#paragraph2)
    1. [Background](#subparagraph2-1)
    2. [Population dynamics](#subparagraph2-2)
    3. [Migration update](#subparagraph2-3)

{% capture text %}
<a name="paragraph1"></a>
#### An eco-evolutionary stoichiometry food-web model of the plankton community 
{% endcapture %}
{% include alert.html text=text color=secondary %}
Advisor: Dr. Shaopeng Wang<br/>
*The Theoretical Ecology Lab, Peking University, Beijing*

##### Model setup<a name="subparagraph1"></a>
{% include figure.html img="plankton model illustration.png" alt="model illustration" caption="2-level food-chain model with stoichiometric constraints indicated in red.<br/>This system is assumed to be carbon sufficient and closed in terms of N and P." width="85%" %}
{% include figure.html img="equations.png" alt="model equations" caption="Model equations<br/>i:N,P; j:zooplankton; k:phytoplankton" width="90%" %}

*Uptake*: there is a linear trade-off between phytoplankton's investment in N update and P uptake, indicated by p_N + p_P = 1. An increase in the relative investment in N uptake (p_N) would meanwhile correspond to a decrease in the relative investment in P uptake. In the model, it is also assumed that this uptake trade-off trait p_N can be an evolving trait, depending on parameter V. V is the genetic variance of this trait, and V = 0 means this trait can't evolve at all. 

*Growth of phytoplankton*: it is limited by the limiting element. 

*Grazing*: besides the maximum grazing rate and predation half saturation constant, the grazing rate of zooplankton also depends on the cell element ratio difference between zooplankton and phytoplankton (i.e., nutritional quality). The probability that zooplankton will consume encountered phytoplankton follows a Gaussian distribution, whose width depends on the grazing selectivity of zooplankton. A higher selectivity gives a more narrow distribution, reducing the probability of grazing on lower quality phytoplankton. The grazing probability is maximized when the consumer and producer have the same N:P ratio.

*Assimilation efficiency*: zooplankton's assimilation efficiency of ingested phytoplankton is assumed to be the lowest ratio of nutrient content of phytoplankton to nutrient content of zooplankton.

**Not only the nutrient availability is important for these processes, the relative amount of different elements also matters**. Such constraints are shown in red in the equations. It can be seen that it is "everywhere".

##### Model extension<a name="subparagraph2"></a>
{% include figure.html img="multiple zooplankton or phytoplankton illustration.png" alt="multiple zooplankton or phytoplankton illustration" caption="Model extension - more species within each trophic level" width="90%" %}

Given the single consumer-single producer model, it is natural to wonder whether two zooplankton could coexist in this system. If two zooplankton have different nutrition demands - one is N-demanding, the other is P-demanding, can they coexist on one species of phytoplankton? It might happen based on a theoretical prediction (`Loladze et al. 2004 - Theor. Popul. Biol.`), that is stable coexistence might occur due to a balance between food quality and quantity.

If the two zooplankton can actually coexist, will that enhance the coexistence of multiple phytoplankton as well? Because aside from phytoplankton competing for resources, there also exists apparent competition between phytoplankton enabled by the existence of zooplankton. One resource and one zooplankton could promote the coexistence of two phytoplankton if there are trade-offs between these two phytoplankton regarding to resources and grazing. Therefore, it is reasonable to predict that 2 resources and 2 zooplankton might be able to maintain the coexistence of more phytoplankton. And the coexistence of these phytoplankton can in turn support two zooplankton as well.

##### Questions to answer<a name="subparagraph3"></a>
{% include figure.html img="BEF stoichiometry framework.png" alt="BEF stoichiometry framework illustration" caption="A conceptual framework of the stoichiometric relationship between biodiversity and ecosystem functioning (BEF) in a trophically structured community. H. Hillebrand et al., BAAE." width="90%" %}

Inspired by the concepts illustrated in the diagram above ```(H. Hillebrand et al., BAAE)```, there are two main questions I hope to answer with this model from a stoichiometry perspective:
1. Coexistence question
 - Under different combinations of N,P availability and ratio, can different zooplankton and phytoplankton coexist?
 - Will the evolution of phytoplankton's uptake trait affect coexistence?
 - How will the variation and variability of parameters like maximum & minimum cell element quota and grazing selectivity affect coexistence?<br/>
 - These questions can be summarized into one question - what is the mechanism of coexistence and what role does stoichiometry play in it?

2. Biodiversity and Ecosystem Functioning (BEF) question
 - Whether biodiversity could enhance the flux of C(energy)/N/P and transfer efficiency?
 - Is the effect of biodiversity on ecosystem functioning mediated by stoichiometry in some way?<br/>

Besides, I am curious what would happen if the strict dichotomy between autotroph and heterotroph is removed. I will further extend the model to allow mixotrophy to investigate it.

##### Example results<a name="subparagraph4"></a>
{% include figure.html img="TE3.png" alt="Transfer efficiency under different nutrient supply and single or two zooplankton comparison" caption="Zooplankton diversity and different nutrient supply on transfer efficiency" width="95%" %}
{% include figure.html img="phyto to zoo flux3.png" alt="producer to consumer flux under different nutrient supply and single or two zooplankton comparison" caption="Zooplankton diversity and different nutrient supply on flux between phytoplankton and zooplankton" width="95%" %}

- Energy transfer efficiency is much lower than element transfer efficiency; carbon flux is much higher than element flux between consumer and producer.
- The diversity of consumers can enhance transfer efficiency while it doesn't necessarily enhance the flux from phytoplankton to zooplankton.
- Increasing N,P input doesn't necessarily promote transfer efficiency but in general could promote the flux.
- C and N transfer efficiencies have fairly similar contour shapes while P's contours are relatively distinct, i.e., the N and P supplies that maximize C and N transfer efficiencies don't necessarily maximize the P transfer efficiency.
- The flux from resource to phytoplankton has similar patterns as the flux from phytoplankton to zooplankton (results not shown).

{% include figure.html img="flux and TE comparison.png" alt="TE and flux comparison between elements and different producer/consumer diversity" caption="Transfer efficiency and flux comparison between elements and different producer/consumer diversity at intermediate N, P supply" width="95%" %}

- Increasing the diversity of consumer and producer in sequence, both the transfer efficiency and the flux between producer and consumer regardless of element first increase and then decline, while the flux into producer decreases all the way.
- I didn't expect the decrease in both fluxes when adding more producers. Working on figuring out why by simulation and analytical analysis!

[Go to top](#top)

{% capture text %}
<a name="paragraph2"></a>
#### A theoretical framework integrating tiger salamander population dynamics and migration across a pond network <br/> 
{% endcapture %}
{% include alert.html text=text color= secondary %}
Advisor: Dr. Dorothy Wallace<br/>
*Department of Mathematics, Dartmouth College, Hanover, NH*

##### Background<a name="subparagraph2-1"></a>
- The pond network is based on the thousands of Isolated shallow playas at Southern high plains. These transient playas could dry out during dry seasons leading to the local extinction of tiger salamander (*Ambystoma tigrinum*).
- Tiger salamander have two forms of adults, metamorphs (terrestrial) and paedomorphs (aquatic).  Upon maturation, juveniles could become either of the forms (i.e., phenotypic plasticity), but only metamorphs have the ability to migrate. 
- Dispersal and recolonization of these transient ponds are essential for the persistence of tiger salamander. 
- I am studying what advantage can phenotypic plasticity contribute to the persistence of this species, and how different morphological choices and different spatial/temporal variations of environment conditions would diversify this contribution.


##### Single pond population dynamics<a name="subparagraph2-2"></a>
{% include figure.html img="single pond population dynamics illustration.png" alt="single pond population dynamics" caption="One circle update of single pond population" width="75%" %}
{% include figure.html img="population update table.png" alt="population update table" caption="Population dynamics at each discrete time step in one circle update" width="80%" %}
{% include figure.html img="population update equations.png" alt="single pond population update equations" caption="One circle update of single pond adult population" width="65%" %}

- We assume that youth of the year and juveniles mature quickly into adults so that there are only adults after each update.  
- The exponent tau of the carrying capacity term (tau << 1) was added in order to prevent from overshooting. If the paedomorph abundance in a pond overshoots the carrying capacity, then the paedomorph abundance might become negative at the next time step.

##### Migration update<a name="subparagraph2-3"></a>
{% include figure.html img="migration illustration.png" alt="migration illustration" caption="Migration across a network of ponds (blue: permanent pond)" width="45%" %}
**Migration update algorithm**:
- Simplified model (no population dynamics involved; `D. Wallace et al. 2014 - Appl. Math. Comput.`)
	- Find all unpopulated ponds, then for each one of them, identify all its near ponds and the distances in between. Calculate the overall probability of updating one unpopulated node to populated (i.e., the probability that at least one populated neighbor pond would migrate to the pond of interest) based on the migration probability and the distance.
	- Find all populated ponds, determine whether to update each of them to unpopulated based on the extinction probability.

In order to make the migration process more realistic, I integrated the population dynamics in each pond into the migration process.
- Integrated model (population dynamics incorporated)
	- Within pond population update (including extinction).
	- Find all ponds that have metamorphs, independently determine whether the metamorphs in each of these ponds will migrate at this step based on the migration probability.
	- If does migrate, randomly choose which neighbor pond will receive these metamorphs, with probability inversely proportional to the distance between the departure pond and the recipient pond.
	- All metamorphs in the departure pond migrate to the recipient neighbor pond, i.e., there will be no more terrestrial adults in the departure pond at this step. 
	- Next within pond population update (including extinction).
   
**Illustration**:
{% include modal.html button="&nbsp; Migration video &nbsp;" color="info" title="Illustration videos" text="I am working on embedding the videos!" %}
<!--
continuous model:
equilibrium has feasibility? 
the time taken to become equilibrium, if too long might cause to extinction, allee effect
-->

[Go to top](#top)
