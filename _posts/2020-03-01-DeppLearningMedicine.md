# Deep learning to fight drug-resistant bacteria

Machine learning has been successfully applied to physics problem since a few years already, 
so much that [Nature](https://www.nature.com/) has already published a 
[review on the topic](https://www.nature.com/articles/s41524-019-0221-0)! 
I am not aware of what exactly is the status in medecine<sup>[1](#myfootnote1)</sup> but I have heard all my friends/relatives 
who are ***real doctors*** worringly discuss the growing issue of drug-resistant infections, so here is a shout-out to them all: AI came in our rescue!

Following a process that reminded me of 
[this](https://www.researchgate.net/publication/334209824_Unsupervised_word_embeddings_capture_latent_knowledge_from_materials_science_literature) 
work<sup>[2](#myfootnote2)</sup>, researches in MIT have used a [deep neural network model to identify new antibiotics](https://www.cell.com/cell/fulltext/S0092-8674(20)30102-1).
They investigated a library of 6'111 molecules, computing prediction scores for each compound so that molecules could be ranked according to their probability of inhibiting *E. coli* growth. 
They removed the compounds used to train their model and empirically tested the 99 molecules with highest prediction scores, finding 51 of these molecules to effectively inhibit *E. coli* growth, with higher prediction scores correlated with a greater probability of growth inhibition<sup>[3](#myfootnote3)</sup>.
Among these 51, they prioritized predicted compounds in preclinical or Phase 1/2/3 studies, those with low structural similarity to training set molecules<sup>[4](#myfootnote4)</sup>, and those with low predicted toxicity. Through this elimination process, emerged ***“halicin”*** (a preclinical nitrothiazole<sup>[5](#myfootnote5)</sup> under investigation as a treatment for diabetes, renamed after *Hal9000* the astronaut-bothering AI in *2001: A Space Odyssey*). 

Halicine was then tested against antibiotic-tolerant *E. coli*, on which had unchanged effectiveness, as well as other drug-resistant bacteria. Halicin was found to be rapidly bactericidal against Mycobacterium tuberculosis and strains of Enterobacteriaceae that are resistant to carbapenems - a group of antibiotics that are considered the last resort for such infections. Halicin also cleared C difficile and multidrug-resistant Acinetobacter baumannii infections.

<iframe width="900" height="506" src="https://www.youtube.com/embed/xZbcwi7SfZE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<a name="myfootnote1">1</a> altough for sure image processing constitutes a great diagnostical opportunity and applications must be blooming.

<a name="myfootnote2">2</a> and was most probably used on many others.

<a name="myfootnote3">3</a> at the same time, tests on the lowest predicted 63 molecules found only two among these compounds to display growth inhibitory activity.

<a name="myfootnote4">4</a> by focusing on compounds that looked effective while structurally different from existing antibiotics (used in the training set), the researchers hoped to find drugs working in radical new ways so that bugs wouldn't have resistance against them.

<a name="myfootnote5">5</a> for those with a knack for medecine: c-Jun N-terminal kinase inhibitor SU3327.
