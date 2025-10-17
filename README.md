# VeriRAG: Knowledge Graph-Augmented RAG for Verilog and Assertions

VeriRAG is an **open-source framework** that unifies **Knowledge Graphs (KG)** and **Retrieval-Augmented Generation (RAG)** for intelligent Verilog automation. It enables semantic understanding, retrieval, and generation of **Register Transfer Level (RTL)** and **System Verilog Assertions (SVA)** code using Large Language Models (LLMs), RDF (Resource Description Framework) graphs, and vector databases. Additional information and paper can be found [here](https://mason.gmu.edu/~rsaravan/projects/VeriRAG.html). 
cff-version: 1.2.0
message: "If you use this software, please cite it as below."
authors:
- family-names: "Lisa"
  given-names: "Mona"
  orcid: "https://orcid.org/0000-0000-0000-0000"
- family-names: "Bot"
  given-names: "Hew"
  orcid: "https://orcid.org/0000-0000-0000-0000"
title: "My Research Software"
version: 2.0.4
doi: 10.5281/zenodo.1234
date-released: 2017-12-18
url: "https://github.com/github-linguist/linguist"
preferred-citation:
  type: article
  authors:
  - family-names: "Lisa"
    given-names: "Mona"
    orcid: "https://orcid.org/0000-0000-0000-0000"
  - family-names: "Bot"
    given-names: "Hew"
    orcid: "https://orcid.org/0000-0000-0000-0000"
  doi: "10.0000/00000"
  journal: "Journal Title"
  month: 9
  start: 1 # First page number
  end: 10 # Last page number
  title: "My awesome research software"
  issue: 1
  volume: 1
  year: 2021
---

## 🚀 Features

- **Knowledge Graph Construction**  
  Converts Verilog RTL into RDF triples (modules, ports, signals, operations) for structured reasoning.

- **ChromaDB Vector Store**  
  Stores semantic embeddings using OpenAI’s `text-embedding-3-small` model for high-precision retrieval.

- **Hybrid Retrieval (SPARQL + Vectors)**  
  Combines symbolic SPARQL queries with semantic similarity search for accurate context retrieval.

- **Prompt Builders for RTL & SVA**  
  Generates context-aware prompts for synthesizing Verilog RTL or SystemVerilog Assertions.

---

## 🧩 Architecture Overview
Dataset (Verilog / CSV)  
↓  
PyVerilog Parsing  
↓  
RDF Knowledge Graph (.ttl)  
↓  
OpenAI Embeddings → ChromaDB  
↓  
Hybrid Retrieval (SPARQL + Vector)  
↓  
Prompt Builder  
↓  
LLM (GPT-4o)  
↓  
Verilog RTL / SVA Generation



---

## 📄 Citation

If you use VeriRAG in your research, please cite:
@inproceedings{verirag-aspdac,
  title={VeriRAG: A Knowledge Graph-Augmented RAG for Verilog and Assertion Generation},
  author={Jayanth ,Thangellamudi and Saravanan, Raghul and Sai Manoj, P D},
  url = {Paper=https://mason.gmu.edu/~rsaravan/papers/VeriRAG.pdf         URL=https://mason.gmu.edu/~rsaravan/projects/VeriRAG.html},

  booktitle={IEEE/ACM ASP-DAC},
  year={2026}
}




