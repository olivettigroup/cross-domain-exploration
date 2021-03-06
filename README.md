### Cross domain exploration
Repository accompanying paper for conducting cross domain exploration of scientific papers: 

**Title**: Augmenting Scientific Creativity with Retrieval across Knowledge Domains

**Authors**: Hyeonsu B Kang, Sheshera Mysore, Kevin J Huang, Haw-Shiuan Chang, Thorben Prein, Andrew McCallum, Niki Kittur, Elsa Olivetti

**Abstract**: Exposure to ideas in domains outside a scientist's own may benefit her in reformulating existing research problems in novel ways and discovering new application domains for existing solution ideas. While improved performance in scholarly search engines can help scientists efficiently identify relevant advances in domains they may already be familiar with, it may fall short of helping them explore diverse ideas outside such domains. In this paper we explore the design of systems aimed at augmenting the end-user ability in cross-domain exploration with flexible query specification. To this end, we develop an exploratory search system in which end-users can select a portion of text core to their interest from a paper abstract and retrieve papers that have a high similarity to the user-selected core aspect but differ in terms of domains. Furthermore, end-users can `zoom in' to specific domain clusters to retrieve more papers from them and understand nuanced differences within the clusters. Our case studies with scientists uncover opportunities and design implications for systems aimed at facilitating cross-domain exploration and inspiration. 

The paper can be accessed here: https://arxiv.org/abs/2206.01328

### Contents
1. [Repository Contents](#repocontents)
1. [Citation](#citation)
1. [TODOs](#todos)


### Repository Contents <a name="repocontents"></a>

`domain-dataset`: Dataset of about 36k papers accompanied with keywords indicative of the sub-domain of the paper. Details of the dataset are described in the accompanying `datasheet.md`.

### Citation <a name="citation"></a>

Please cite the paper as:  

```bibtex
@inproceedings{naacl2022_kang_augmenting,
      title={Augmenting Scientific Creativity with Retrieval across Knowledge Domains},
      author={Kang, Hyeonsu B and Mysore, Sheshera and Huang, Kevin J and Chang, Haw-Shiuan and Prein, Thorben and McCallum, Andrew and Kittur, Aniket and Olivetti, Elsa},
      booktitle={Second Workshop on Bridging Human-Computer Interaction and Natural Language Processing at NAACL 2022},
      year={2022}
    }
```

### Todo <a name="todo"></a>

1. Release code for the system described in the paper.