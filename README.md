# VeriRAG: Knowledge Graph-Augmented RAG for Verilog and Assertions

VeriRAG is an **open-source framework** that unifies **Knowledge Graphs (KG)** and **Retrieval-Augmented Generation (RAG)** for intelligent Verilog automation. It enables semantic understanding, retrieval, and generation of **Register Transfer Level (RTL)** and **System Verilog Assertions (SVA)** code using Large Language Models (LLMs), RDF (Resource Description Framework) graphs, and vector databases. Additional information and paper can be found [here](https://mason.gmu.edu/~rsaravan/projects/VeriRAG.html). 

If you find this paper as useful, please cite as:
@inproceedings{verirag-aspdac,
  title={VeriRAG: A Knowledge Graph-Augmented RAG for Verilog and Assertion Generation},
  author={Jayanth ,Thangellamudi and Saravanan, Raghul and Sai Manoj, P D},
  booktitle={IEEE/ACM ASP-DAC},
  year={2026}



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


}




