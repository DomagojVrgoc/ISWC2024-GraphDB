# Recent advances in Graph Data Management

Author: Domagoj Vrgoč

Details: [preprint](https://raw.githubusercontent.com/DomagojVrgoc/ISWC2024-GraphDB/main/ISWC_Tutorial.pdf)

## Abstract and motivation:
Graph databases have received a lot of attention in recent years, mostly due to their role as the underlying storage and query mechanism for knowledge graphs. This led to different graph solution being developed throughout the years, with the RDF data format together with the SPARQL query standard being widely used in large open knowledge graphs such as Wikidata or DBpedia, while commercial systems generally deploy the property graph data model, with the recent GQL ISO standard formalizing query languages in this setting. In this tutorial we give a detailed overview of graph data models and query standards, followed by a deep dive into recent techniques for graph query processing, most notably the use of worst-case optimal algorithms and automata-guided path retreival. Overall, the tutorial will be aiming to answer the question of what is needed to effectively manage large knowledge graphs and how helpful how much are recent developments in database research in this regard.

## Schedule:
The tutorial is divided into four largely independent sections. In the first section we will introduce attendees to popular graph data models and query languages and try to bridge the gap between RDF and property graphs, opening the floor to discussion on the appropriate formalism for representing knowledge graphs. The second section will overview worst-case optimal algorithms, a recent advancement in join processing, and show how this theoretical concept can be adapted in practice to evaluate basic graph patterns. The third section deals with path queries and shows how to adapt an old idea from database theory to efficiently compute a representation of a potentially exponential set of paths in linear time. In the final section we introduce MillenniumDB, a system build on these ideas with the goal of managing Wikidata and discuss what it takes to make theory work in practice at this scale. Apart from the open discussion sessions, the interactive portion of the tutorial will also include a series of endpoints hosted in MillenniumDB and allowing to try these techniques over different RDF and property graph datasets.
## Endpoint details (in preparation):

### SPARQL Endpoints:

#### Full Wikidata (RDF/SPARQL): [https://wikidata.imfd.cl/](https://wikidata.imfd.cl/)

#### Wikidata Truthy (RDF/Extended SPARQL): [https://mdb.imfd.cl/path_finder/sparql](https://mdb.imfd.cl/path_finder/sparql)

### Property graph endpoints:

#### Wikidata Truthy: [https://mdb.imfd.cl/path_finder/gql](https://mdb.imfd.cl/path_finder/gql)

#### BibKG: [https://bibkg.imfd.cl/](https://bibkg.imfd.cl/)

#### TelarKG: [https://telarkg.imfd.cl/](https://telarkg.imfd.cl/)

## Slides:
In preparation ... 

## References
1. Aidan Hogan, Eva Blomqvist, Michael Cochez, Claudia d'Amato, Gerard de Melo, Claudio Gutierrez, Sabrina Kirrane, José Emilio Labra Gayo, Roberto Navigli, Sebastian Neumaier, Axel-Cyrille Ngonga Ngomo, Axel Polleres, Sabbir M. Rashid, Anisa Rula, Lukas Schmelzeisen, Juan F. Sequeda, Steffen Staab, Antoine Zimmermann: Knowledge Graphs. ACM Comput. Surv. 54(4): 71:1-71:37 (2022)
2. Aidan Hogan: The Web of Data. Springer 2020, ISBN 978-3-030-51579-9, pp. 1-642
3. Renzo Angles, Marcelo Arenas, Pablo Barceló, Aidan Hogan, Juan L. Reutter, Domagoj Vrgoč: Foundations of Modern Query Languages for Graph Databases. ACM Comput. Surv. 50(5): 68:1-68:40 (2017)
4. Albert Atserias, Martin Grohe, Dániel Marx: Size Bounds and Query Plans for Relational Joins. SIAM J. Comput. 42(4): 1737-1767 (2013)
5. Hung Q. Ngo, Christopher Ré, Atri Rudra: Skew strikes back: new developments in the theory of join algorithms. SIGMOD Rec. 42(4): 5-16 (2013)
6. Benjamín Farias, Wim Martens, Carlos Rojas, Domagoj Vrgoč: Evaluating Regular Path Queries in GQL and SQL/PGQ: How Far Can The Classical Algorithms Take Us? CoRR abs/2306.02194 (2023)
7. Domagoj Vrgoč, Carlos Rojas, Renzo Angles, Marcelo Arenas, Diego Arroyuelo, Carlos Buil-Aranda, Aidan Hogan, Gonzalo Navarro, Cristian Riveros, Juan Romero: MillenniumDB: An Open-Source Graph Database System. Data Intell. 5(3): 560-610 (2023)
