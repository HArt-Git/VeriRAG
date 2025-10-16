# VeriRAG: Knowledge Graph-Augmented RAG for Verilog and Assertions

VeriRAG is an **open-source framework** that unifies **Knowledge Graphs (KG)** and **Retrieval-Augmented Generation (RAG)** for intelligent Verilog automation.  
It enables semantic understanding, retrieval, and generation of **RTL** and **SVA** code using LLMs, RDF graphs, and vector databases.

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





