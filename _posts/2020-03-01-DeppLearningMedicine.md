# Deep learning to fight drug-resistant bacteria

Machine learning has been successfully applied to physics problem since a few years already, 
so much that [Nature](https://www.nature.com/) has already published a 
[review on the topic](https://www.nature.com/articles/s41524-019-0221-0)! 
I am not aware of what exactly is the status in medecine<sup>[1](#myfootnote1)</sup> but I have heard all my friends/relatives 
who are ***real doctors*** worringly discuss the growing issue of drug-resistant infections, so here is a shout out to them all: AI came to our rescue!

Following a process that reminded me of [this](https://www.researchgate.net/publication/334209824_Unsupervised_word_embeddings_capture_latent_knowledge_from_materials_science_literature) work<sup>[2](#myfootnote2)</sup>, researches in MIT have used a [deep neural network model to identify new antibiotics](https://www.cell.com/cell/fulltext/S0092-8674(20)30102-1).
They investigated a library of 6'111 molecules, computing prediction scores for each compound so that molecules could be ranked according to their probability of inhibiting *E. coli* growth. 
They removed the compounds used to train their model and empirically tested the 99 molecules with highest prediction scores, finding 51 of these molecules to effectively inhibit *E. coli* growth, with higher prediction scores correlated with a greater probability of growth inhibition<sup>[3](#myfootnote3)</sup>.
Among these 51, they prioritized compounds in preclinical studies, those with low structural similarity to training set molecules<sup>[4](#myfootnote4)</sup>, and those with low predicted toxicity. 
Through this elimination process, emerged ***“halicin”*** (a preclinical nitrothiazole<sup>[5](#myfootnote5)</sup> under investigation as a treatment for diabetes, renamed after *Hal9000* the astronaut-bothering AI in *2001: A Space Odyssey*). 

Halicine was then tested against antibiotic-tolerant *E. coli*, on which had unchanged effectiveness, as well as other drug-resistant bacteria and it was found to be a **broad-spectrum bactericidal antibiotic with exceptional in vivo efficacy**<sup>[6](#myfootnote6)</sup>.
The researchers have already moved to explore a larger dataset (comprising more than 107 MILLION compounds), identifying two more molecules that display broad-spectrum activity and maintain activity against antibiotic-tolerant *E. coli*. 

While [The Guardian](https://www.theguardian.com/society/2020/feb/20/antibiotic-that-kills-drug-resistant-bacteria-discovered-through-ai) discusses these results in a more lenghty yet accessible way, I'd like to stress what an accomplishment this algorithm represents. 
Halicine might have never reached clinical trials, and even then its bactericidal properties might have been overlooked or listed among adverse side effects. 
107 million compounds, or even 'just' 6 thousands, would require an enormous amount of time and money to traditionally explore. 
Furthermore, the availability of such a tool might even allow for antibiotic 'engineering'.
Machine learning has enabled a new fast promising route towards solving a complicated important and scary problem, and leaves me wonder about its incredible potential for applications in so many different fields: will it be solving problems that we don't even know we have yet? I guess, the sky is the limit.
 
   <br>

<iframe width="680" height="470"  src="https://www.youtube.com/embed/xZbcwi7SfZE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
 
   <br>

<a name="myfootnote1">1</a> altough for sure image processing constitutes a great diagnostical opportunity and applications must be blooming.

<a name="myfootnote2">2</a> and was most probably used on many others.

<a name="myfootnote3">3</a> at the same time, tests on the lowest predicted 63 molecules found only two among these compounds to display growth inhibitory activity.

<a name="myfootnote4">4</a> by focusing on compounds that looked effective while structurally different from existing antibiotics (used in the training set), the researchers hoped to find drugs working in radical new ways so that bugs wouldn't have resistance against them.

<a name="myfootnote5">5</a> for those with a knack for medecine: c-Jun N-terminal kinase inhibitor SU3327.


<a name="myfootnote6">6</a> in patient samples, halicin was found to be rapidly bactericidal against Mycobacterium tuberculosis and strains of Enterobacteriaceae that are resistant to carbapenems - a group of antibiotics that are considered the last resort for such infections. Halicin also cleared C difficile and multidrug-resistant Acinetobacter baumannii infections in mice.
