# Inferring CAD Modeling Sequences using Zone Graphs

## Release Notes
The official implementation of [Zone Graph](http://pwz.mit.edu/projects/ZG/), published at CVPR 2021. 
<img src="teaser-image.png" alt="drawing" width="80%"/>

In computer-aided design (CAD), the ability to "reverse engineer" the modeling steps used to create 3D shapes is a long-sought-after goal. This process can be decomposed into two sub-problems: converting an input mesh or point cloud into a boundary representation (or B-rep), and then inferring modeling operations which construct this B-rep. In this paper, we present a new system for solving the second sub-problem. Central to our approach is a new geometric representation: the zone graph. Zones are the set of solid regions formed by extending all B-Rep faces and partitioning space with them; a zone graph has these zones as its nodes, with edges denoting geometric adjacencies between them. Zone graphs allow us to tractably work with industry-standard CAD operations, unlike prior work using CSG with parametric primitives. We focus on CAD programs consisting of sketch + extrude + Boolean operations, which are common in CAD practice. We phrase our problem as search in the space of such extrusions permitted by the zone graph, and we train a graph neural network to score potential extrusions in order to accelerate the search. We show that our approach outperforms an existing CSG inference baseline in terms of geometric reconstruction accuracy and reconstruction time, while also creating more plausible modeling sequences.


## Running Zone Graph

More code is comming !

See [this link](./src) for instructions of running the code.

## Citation
Please cite the following paper if you find the code useful for your research/projects.

```
@inproceedings{,
  author    = "Xianghao Xu and Wenzhe Peng and Chin-Yi Cheng 
               and Karl D. D. Willis and Daniel Ritchie",
  title     = "Inferring CAD Modeling Sequences Using Zone Graphs",
  booktitle = "CVPR",
  year      = "2021"
}
```
