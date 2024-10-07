# Results


## Experimental results

### Is phage propagation dependent on the selection phage? 
We tested if the E3 ligases SIAH1 and SIAH2 can trigger phage replication when a specific target protein is present. We used the protein EGLN3, which is known to be recognised by SIAH1 and SIAH2. We attached EGLN3 to part of the T7 RNA polymerase enzyme and infected cells with a few phages carrying the SIAH1 or SIAH2 gene. We measured the amount of phage produced after incubating the cells overnight. The phages carrying SIAH1 and SIAH2 replicated more than phages with an unrelated protein. This experiment indicates that our system worked.


<figure markdown>
![Figure_initial_difference](https://idec-teams.github.io/2024_Evolution_Suisse/img/result figures/Boxplot_quality_positions_wiki.png)
<figcaption> Phages carrying SIAH1 or SIAH2 grow much better than phages carrying an unrelated protein. The fold change shows how much the number of phages increased or decreased (If the number of phages doubles, that is a two-fold increase).</figcaption>
</figure>

We then looked at whether changing the target protein affects phage replication. We replaced EGLN3 (blue) with α-Synuclein (orange), which is also recognised by SIAH1/2. Changing the target protein changes the level of phage propagation. This shows that our system depends on SIAH1 or SIAH2 and the target protein interacting together. 

<figure markdown>
![Figure_initial_difference](https://idec-teams.github.io/2024_Evolution_Suisse/img/result figures/Boxplot_quality_positions_wiki.png)
<figcaption> Phage propagation is dependent on the substrate. The fold change shows how much the number of phages increased or decreased. </figcaption>
</figure>
 

Next, we looked at how changes in the degron would affect our system. We found that even when we altered key parts of the degron in EGLN3, phage replication was not significantly affected. This suggests that phage propagation might be triggered by other factors than the degron. 

<figure markdown>
![Figure_degron_dependency](https://idec-teams.github.io/2024_Evolution_Suisse/img/result figures/Boxplot_quality_positions_wiki.png)
<figcaption> Phage propagation is not affected by the disruption of the degron. The wildtype degron is: FIADVEP. The fold change shows how much the number of phages increased or decreased. </figcaption>
</figure>

We were able to show that phage propagation is dependent on both the substrate of the E3 ligase and the E3 ligase itself. However, we also observed a very high background phage propagation in our system. For our evolution to work, we need to be able to link phage proliferation to degron recognition, so this phage proliferation caused by other factors than the degron interferes with the use of this system for the directed evolution part of this project. The next step is to find out why this is happening and how we can modify our system so that it doesn't happen. 

### What factors lead to unwanted, E3-ligase independent page propagation? 
We suspected that the background phage propagation we observed could be caused by one of two things: 
Leaky transcription of gIII: the gene controlling phage growth is turned on without the split-RNAP components being present. 
Spontaneous assembly of the split-RNAP subunits: The two halves of the RNAP are coming together on their own, without the need of ubiquitination of the target substrate. 

Both hypotheses lead to gIII expression independent of the E3 ligase activity. To test these hypotheses, we quantified phage propagation in cells that had only one half of the RNAP. In these cells, phage propagation was suppressed, confirming that both halves of the RNAP are required to activate gIII expression. This means that accidental activation of gIII wasn’t the issue. Instead, these results show that the two enzyme halves were probably joining together on their own, causing phage propagation without the involvement of the E3 ligase.

<figure markdown>
![Figure_split_RNAP_parts](https://idec-teams.github.io/2024_Evolution_Suisse/img/result figures/Boxplot_quality_positions_wiki.png)
<figcaption> Phage propagation in the presence and absence of split-RNAP components. This figure shows how much the phage population changed after overnight incubation with bacteria missing one of the two halves of the split-RNAP. The results are shown as a log2-fold change, meaning the numbers show how much the phage count increased or decreased, compared to the starting level. NC (negative control) is a bacterial strain lacking both parts of the system. PC (positive control) is a bacterial strain with the full system.</figcaption>
</figure>

We observed that the RNAP enzyme can assemble and become active before the phages even enter the bacterial cells. This early assembly can lead to unwanted phage propagation, which interferes with our goal to link phage propagation to E3 ligase activity. To overcome this problem, we changed the way we control the production of the N- and C-terminal halves of the RNAP. Instead of using a constitutive promoter, which is always active and produces the protein, we switched to a promoter that can be turned on when needed. For this, we chose two different inducible systems. One is switched on by adding vanillic acid (pVan promoter), the other by the stress response caused by phage infection (phage shock promoter). These new systems let us delay the production of the RNAP halves until just before or during phage infection. By regulating when these components are expressed, we can reduce the unintended assembly of the RNAP. This method can easily be added to the PACE system, allowing precise control of the timing of RNAP production.

### Enhancing SIAH1 genetic diversity using drift. 

During PACE, both phages and infected bacteria are continuously removed from the lagoon. If phages propagate too slowly there's a risk that all the phages could be washed out before they can replicate and evolve. This is especially risky at the start of the experiment, when the initial activity of the E3 ligase may be too low to maintain sufficient phage propagation. To mitigate this risk, a process called "drift" is used before the evolution starts. Drift allows random mutations to occur without any selection pressure, increasing the genetic diversity among the phages. This genetic variability helps prevent phage washout by giving the population a better chance of harbouring variants with higher activity that can sustain propagation in the lagoon.

To this end, we propagated the SIAH1 SP phages in bacterial cells that contain a special drift plasmid (DP6). The DP6 plasmid not only increases the mutation rate but also supplies the necessary pIII protein, allowing phages to replicate regardless of the E3 ligase's activity. Over eight infection and growth cycles (called passages), we sequenced the SIAH1 SP phages, and estimated the amount of mutations at different positions in the SIAH1 gene. With each passage, we saw the number of mutated phages increase, creating a highly diverse pool of SIAH1 SP phages. This pool can then serve as a robust starting pool for the next stages of evolutionary experiments, reducing the risk of phage washout and enhancing the chances of evolving phages with improved E3 ligase activity.

<figure markdown>
![Figure_SIAH1_drift](https://idec-teams.github.io/2024_Evolution_Suisse/img/result figures/Boxplot_quality_positions_wiki.png)
<figcaption> Detection of mutated bases in SIAH1-SP during eight drift passages This figure illustrates the accumulation of mutations in the SIAH1-SP gene across eight cycles of drift. Each cycle represents one passage, during which the phages underwent random mutations in the absence of selection pressure. The data demonstrate how much genetic variation has been introduced over the course of the drift passages</figcaption>
</figure>

