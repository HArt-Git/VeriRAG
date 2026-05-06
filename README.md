# VeriRAG: Knowledge Graph-Augmented RAG for Verilog and Assertions

VeriRAG is an **open-source framework** that unifies **Knowledge Graphs (KG)** and **Retrieval-Augmented Generation (RAG)** for intelligent Verilog automation. It enables semantic understanding, retrieval, and generation of **Register Transfer Level (RTL)** and **System Verilog Assertions (SVA)** code using Large Language Models (LLMs), RDF (Resource Description Framework) graphs, and vector databases. Additional information and paper can be found [here](https://mason.gmu.edu/~rsaravan/projects/VeriRAG/VeriRAG.html). 

If you find this paper as useful, please cite as:

@INPROCEEDINGS{11420790,
  author={Thangellamudi, Jayanth and Saravanan, Raghul and Dinakarrao, Sai Manoj Pudukotai},
  booktitle={2026 31st Asia and South Pacific Design Automation Conference (ASP-DAC)}, 
  title={VeriRAG: A Knowledge Graph-Augmented RAG for Verilog and Assertion Generation}, 
  year={2026},
  volume={},
  number={},
  pages={105-111},
  keywords={Design automation;Semantics;Retrieval augmented generation;Knowledge graphs;Syntactics;Hybrid power systems;Hardware;Vectors;Hardware design languages;Standards},
  doi={[10.1109/ASP-DAC66049.2026.11420790](https://doi.org/10.1109/ASP-DAC66049.2026.11420790)}}




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
## Prerequisites
- This notebook is designed for Google Colab environments (mounts Google Drive under /content/drive)
- You must provide a valid OpenAI API key
- You should have a CSV file compatible with the expected schema (see Section 7 in the code for details).

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
      LLM   
       ↓  
Verilog RTL / SVA Generation



---






