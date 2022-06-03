Following recommended practice to report the details of the dataset, we provide a Datasheet following prompts provided in [Bender et. al. 2018](https://www.aclweb.org/anthology/Q18-1041/) and [Gebru et. al. 2018](https://arxiv.org/abs/1803.09010).

### Motivation

Q: For what purpose was the dataset created?    
A: The dataset was created as an evaluation set to compare the suitability of different approaches to cluster scientific research literature into subdomains, in an unsupervised manner.

Q: Who created the dataset and on behalf of which entity?       
A: The dataset was created by researchers at the [Olivetti Group](https://olivetti.mit.edu) at the Department of Materials Science and Engineering at MIT and the [Information Extraction and Synthesis Laboratory](https://www.iesl.cs.umass.edu/) at the University of Massachusetts Amherst on behalf of those same entities. 

Q: Who funded the creation of the dataset?     
A: This work is supported by R.D. Shell.


### Composition

Q: What do the instances that comprise the dataset represent? How many instances are there in total (of each type, if appropriate)?         
A: The dataset includes titles and abstracts of 39699 scientific publication. Each instance is representative of one scientific publication in the field of Materials Science and furthermore a subfield therein. 

Q: Does the dataset contain all possible instances or is it a sample of instances from a larger set?     
A: The dataset is no sample of a publicly available larger dataset. It represents a filtered version of a larger non-public collection of Materials Science papers. This larger collection was set up for a variety of different Materials Science-related projects making it a suitable source for covering a broader range of materials science subfields. The selection of the cluster-defining keywords has been made by the authors, applying their expert knowledge in the field.

Q: Is there a label or target associated with each instance?      
A: Each instance is assigned to a gold cluster. Instances can only be affiliated with one gold cluster and gold clusters are described by their unique list of author provided keyword strings, shared among the publications within the specific cluster.

Q: Is any information missing from individual instances?        
A: The authors are not aware of any missing information among the instances.

Q: Are relationships between individual instances made explicit (e.g., users movie ratings, social network links)?	  
A: The gold cluster labels use author provided keywords of the papers to group related papers in clusters.

Q: Are there recommended data splits (e.g., training, development/validation, testing)?     
A: -

Q: Are there any errors, sources of noise, or redundancies in the dataset?      
A: The dataset was built from abstracts, titles, metadata, and author-provided keywords through filtering of a larger corpus. Due to the nature of automatic extraction individual instances of the dataset may contain incorrect information. Furthermore, the dataset excludes such papers that would be assigned to multiple of the defined Materials Science gold clusters (e.g. multiple keyword matches).   

Q: Is the dataset self-contained, or does it link to or otherwise rely on external resources (e.g., websites, tweets, other datasets)?      
A: The dataset is self contained.

Q: Does the dataset contain data that might be considered confidential?      
A: No.

Q: Does the dataset contain data that, if viewed directly, might be offensive, insulting, threatening, or might otherwise cause anxiety?      
A: No.

Q: Does the dataset relate to people?      
A: The dataset relates to people in-as-much as it consists of research papers the authors of are included as part of the metadata.

Q: Does the dataset identify any subpopulations (e.g., by age, gender)?      
A: No.

Q: Is it possible to identify individuals (i.e., one or more natural per- sons), either directly or indirectly (i.e., in combination with other data) from the dataset?      
A: The authors of individual papers included in the dataset are present as part of metadata. If absent, web searches can easily reveal authors.

Q: Does the dataset contain data that might be considered sensitive in any way?    
A: No.

Q: Speaker demographic and Language Variety following [Bender et al. 2018](https://www.aclweb.org/anthology/Q18-1041/).      
A: The text of the abstracts is primarily academic writing in English.  

Q: Annotator demographics following [Bender et al. 2018](https://www.aclweb.org/anthology/Q18-1041/):       
The dataset was annotated by 2 annotators. 

### Collection Process

Q: What mechanisms or procedures were used to collect the data (e.g., hardware apparatus or sensor, manual human curation, software program, software API)?      
A: The dataset is part of a larger non-public corpus on Materials Science literature at MIT, procedures included various queries through the [LENS API](https://docs.api.lens.org/index.html) and curation of the results in a python 3 environment .

Q: If the dataset is a sample from a larger set, what was the sampling strategy (e.g., deterministic, probabilistic with specific sampling probabilities)?      
A: The sampling strategy aimed to cover a diverse range of different Materials Science subdomains, while excluding papers relating to multiple of the curator-defined subdomains.

Q: Who was involved in the data collection process (e.g., students, crowdworkers, contractors) and how were they compensated (e.g., how much were crowdworkers paid)?      
A: One graduate student and a post-doc. They were not specifically compensated for the work related to setting up the dataset.

Q: Over what timeframe was the data collected?      
A: Three days. 

Q: Were any ethical review processes conducted (e.g., by an institutional review board)?      
A: No. 

Q: Did you collect the data from the individuals in question directly, or obtain it via third parties or other sources (e.g., websites)?      
A: Scientific papers were gathered from different publishers. Relevance judgments were made directly by the dataset authors.

Q: Were the individuals in question notified about the data collection?      
A: Yes.

Q: Did the individuals in question consent to the collection and use of their data?      
A: NA.

Q: If consent was obtained, were the consenting individuals provided with a mechanism to revoke their consent in the future or for certain uses?   
A: No.

Q: Has an analysis of the potential impact of the dataset and its use on data subjects been conducted?    
A: No.   

Q: Was any preprocessing/cleaning/labeling of the data done?    
A: At first, the most frequent author-provided keywords were viewed and then clustered into subtopics by the authors. In a second step papers were assigned to these clusters, excluding papers linking to multiple clusters.

Q: Was the "raw" data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)?     
A: NA.

Q: Is the software used to preprocess/clean/label the instances available?      
A: No.

### Uses

Q: Has the dataset been used for any tasks already?    
A: Yes. It has been used in the publication *Sheshera Mysore, Hyeonsu B Kang, Kevin J Huang, Haw-Shiuan Chang, Thorben Prein, Andrew McCallum, Niki Kittur, Elsa Olivetti, "Augmenting Scientific Creativity with Retrieval across Knowledge Domains", NLP+HCI Workshop at NAACL, 2022 (to appear)*.

Q: Is there a repository that links to any or all papers or systems that use the dataset?      
A: Yes, [here](https://github.com/olivettigroup/cross-domain-exploration).

Q: What (other) tasks could the dataset be used for?    
A: The dataset is intended for the evaluation of different approaches to identify subdomains in the scientific literature in an unsupervised way.

Q: Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses?    
A: None that we are aware of.

Q: Are there tasks for which the dataset should not be used?     
A: None that we can think of.

### Description

Q: Will the dataset be distributed to third parties outside of the entity (e.g., company, institution, organization) on behalf of which the dataset was created?     
A: No.     

Q: How will the dataset will be distributed (e.g., tarball on website, API, GitHub)?      
A: GitHub. Please use the appropriate [release](https://github.com/olivettigroup/cross-domain-exploration) to download salient releases of the dataset.      

Q: When will the dataset be distributed?     
A: The dataset has been publicly available since July 1st 2022.

Q: Will the dataset be distributed under a copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?   
A: The dataset is released under the [Creative Commons Attribution-NonCommercial 4.0 International](https://creativecommons.org/licenses/by-nc/4.0/legalcode) license.

Q: Have any third parties imposed IP-based or other restrictions on the data associated with the instances?     
A: None.

Q: Do any export controls or other regulatory restrictions apply to the dataset or to individual instances?     
A: None.

### Maintenance

Q: Who is supporting/hosting/maintaining the dataset?    
A: Thorben Prein (prein at mit.edu)

Q: How can the owner/curator/manager of the dataset be contacted?    
A: Yes.

Q: Is there an erratum?    
A: None yet.

Q: Will the dataset be updated (e.g., to correct labeling errors, add new instances, delete instances)?    
A: If sufficiently large errors are discovered the dataset will be corrected and updated versions of it will be released. We will use the "Releases" feature on Github to denote all salient releases.