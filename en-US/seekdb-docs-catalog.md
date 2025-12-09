# Seekdb Documentation Catalog

This catalog provides a comprehensive index of all seekdb documentation. When users ask about seekdb-related topics, you can use the descriptions to find relevant documents and fetch the content from the specified URLs.

**Base URL**: `https://github.com/oceanbase/seekdb-doc/tree/V1.0.0/en-US/`

> **Note**: All File Paths below are relative paths. The full URL = Base URL + File Path

---

# Documentation Overview

- **File Path**: `10.doc-overview.md`

  - **Description**: seekdb documentation overview, including quick links to get started guides, SDK references, integrations, and tutorials

---

# Get Started

This category contains quick start tutorials and basic operation guides for the seekdb database.

## Summary

This category contains **11** documentation files covering seekdb quick start, basic operations, feature experiences, and AI application building.

### Seekdb Overview

- **File Path**: `100.get-started/10.overview/10.seekdb-overview.md`

  - **Description**: Introduction to what seekdb is - an AI-native search database that unifies relational, vector, text, JSON and GIS in a single engine, enabling hybrid search and in-database AI workflows. Includes capability matrix, product architecture, core advantages, and applicable scenarios like RAG, AI-assisted programming, semantic search, and agentic AI applications.

### Embedded Mode

- **File Path**: `100.get-started/50.embedded-mode/25.using-seekdb-in-python-sdk.md`

  - **Description**: How to use seekdb in embedded mode with Python SDK (pyseekdb). Covers installation, prerequisites, and basic usage examples including connecting to seekdb, creating collections with embedding functions, adding data, and querying with automatic vector generation.

### Client-Server Mode

- **File Path**: `100.get-started/100.client-server-mode/10.deploy-seekdb-testing-environment.md`

  - **Description**: Quick deployment guide for seekdb in client/server mode using yum install or Docker containers. Includes prerequisites, system requirements, and step-by-step deployment instructions.

- **File Path**: `100.get-started/100.client-server-mode/15.basic-sql-operations.md`

  - **Description**: Basic SQL operations in seekdb including creating databases, table operations (CREATE, ALTER, DROP), index operations, data manipulation (INSERT, DELETE, UPDATE, SELECT), transaction control (COMMIT, ROLLBACK), and user management.

- **File Path**: `100.get-started/100.client-server-mode/30.experience-vector-search.md`

  - **Description**: Guide to experiencing vector search in seekdb. Covers creating vector columns and indexes, inserting vector data, performing vector search using SQL, and comparison between exact search and approximate search using HNSW indexes.

- **File Path**: `100.get-started/100.client-server-mode/40.experience-full-text-indexing.md`

  - **Description**: Guide to experiencing full-text indexing in seekdb. Covers how full-text indexing works with BM25 algorithm, creating full-text indexes with different tokenizers (Beng, IK, space, ngram), Boolean mode queries, and performance comparison with MySQL.

- **File Path**: `100.get-started/100.client-server-mode/50.experience-hybrid-search.md`

  - **Description**: Guide to hybrid search combining vector-based semantic search and full-text keyword search. Covers pure vector search, pure full-text search, hybrid search using DBMS_HYBRID_SEARCH package, and parameter tuning with boost weights.

- **File Path**: `100.get-started/100.client-server-mode/60.experience-ai-function.md`

  - **Description**: Guide to AI function service in seekdb. Covers AI_EMBED for text-to-vector conversion, AI_COMPLETE and AI_PROMPT for text generation with LLMs, AI_RERANK for result reranking, and building an intelligent Q&A system combining all functions.

- **File Path**: `100.get-started/100.client-server-mode/70.experience-hybrid-vector-index.md`

  - **Description**: Guide to hybrid vector indexes that automatically convert text to vectors and build indexes. Covers creating hybrid vector indexes, inserting text data without manual vectorization, and using semantic_distance function for text-based retrieval.

- **File Path**: `100.get-started/100.client-server-mode/80.experience-vibe-coding-paradigm-with-cursor-agent-oceanbase-mcp.md`

  - **Description**: Guide to the Vibe Coding paradigm using Cursor Agent and OceanBase MCP. Covers setting up Cursor with OceanBase MCP Server, configuring database connections, and building RESTful APIs using natural language instructions.

### Build AI Applications

- **File Path**: `100.get-started/150.build-ai-apps/90.build-ai-apps.md`

  - **Description**: Overview page for building AI applications with seekdb, including links to tutorials for building knowledge base applications, cultural tourism assistants with multi-model integration, and image search applications.

---

# Development Guide

This category contains detailed development guides for seekdb features including vector search, hybrid search, AI functions, SDK, and multi-model data support.

## Vector Search

### Vector Search Overview

- **File Path**: `200.develop/100.vector-search/100.vector-search-overview/100.vector-search-intro.md`

  - **Description**: Comprehensive overview of vector search concepts including unstructured data, vectors, vector embedding, vector similarity search, and why choose seekdb for vector search (hybrid retrieval, scalability, high performance, transactions, cost efficiency, data security).

- **File Path**: `200.develop/100.vector-search/100.vector-search-overview/300.vector-search-workflow.md`

  - **Description**: AI application workflow using seekdb vector search, from converting unstructured data to vectors, storing embeddings and creating indexes, performing nearest neighbor and hybrid search, to generating prompts for LLM inference.

### Vector Embedding

- **File Path**: `200.develop/100.vector-search/150.vector-embedding-technology.md`

  - **Description**: Vector embedding technology guide covering what vector embedding is, generating embeddings using AI function service in seekdb, common text embedding methods (Sentence Transformers, Hugging Face, Ollama), and image embedding with CLIP.

### Store Vector Data

- **File Path**: `200.develop/100.vector-search/160.store-vector-data.md`

  - **Description**: How to store vector data in seekdb including creating vector columns with VECTOR data type, and inserting vector data using INSERT statements.

### Vector Indexes

- **File Path**: `200.develop/100.vector-search/200.vector-index/200.dense-vector-index.md`

  - **Description**: Comprehensive guide to dense vector indexes including index types (HNSW, HNSW_SQ, HNSW_BQ, IVF, IVF_PQ, IVF_SQ), memory estimation, creation syntax, maintenance operations, and query examples.

- **File Path**: `200.develop/100.vector-search/200.vector-index/300.hybrid-vector-index.md`

  - **Description**: Guide to creating hybrid vector indexes that automatically embed text. Covers synchronous and asynchronous modes, creation syntax, prerequisites for registering embedding models, and using semantic_distance function.

- **File Path**: `200.develop/100.vector-search/200.vector-index/400.sparse-vector-index/100.in-memory-sparse-vector-index.md`

  - **Description**: Guide to in-memory sparse vector indexes for sparse vector data.

### Vector Functions

- **File Path**: `200.develop/100.vector-search/250.vector-function.md`

  - **Description**: SQL functions for vector operations including distance functions (L2_distance, Cosine_distance, Inner_product), vector arithmetic functions, and normalization functions.

### Vector Similarity Search

- **File Path**: `200.develop/100.vector-search/300.vector-similarity-search.md`

  - **Description**: Vector similarity search guide covering exact nearest neighbor search (full-scan) and approximate nearest neighbor search using vector indexes. Includes examples for Euclidean, cosine, and inner product similarity search.

### Vector Search Reference

- **File Path**: `200.develop/100.vector-search/700.vector-search-reference/100.vector-data-type.md`

  - **Description**: Reference for vector data types in seekdb.

- **File Path**: `200.develop/100.vector-search/700.vector-search-reference/800.vector-sdk-refer.md`

  - **Description**: Reference for vector SDK usage.

### Benchmark and FAQ

- **File Path**: `200.develop/100.vector-search/700.vector-search-benchmark-test.md`

  - **Description**: Guide to benchmark testing with VectorDBBench, including prerequisites, installation, configuration, and running performance tests on seekdb vector database.

- **File Path**: `200.develop/100.vector-search/800.vector-search-faq.md`

  - **Description**: Frequently asked questions about vector search including data dimensionality requirements, maximum rows, and creating indexes on high-dimensional vectors.

## Hybrid Search

- **File Path**: `200.develop/200.hybrid-search/100.vector-index-hybrid-search.md`

  - **Description**: Comprehensive guide to hybrid search with full-text indexes and vector indexes using DBMS_HYBRID_SEARCH package. Covers use cases including scalar search, vector search, full-text search, and various combinations with filtering and sorting.

## AI Function

- **File Path**: `200.develop/300.ai-function/100.ai-function-permission.md`

  - **Description**: AI function privileges guide covering CREATE/ALTER/DROP AI MODEL privileges and ACCESS AI MODEL privileges for calling AI functions.

- **File Path**: `200.develop/300.ai-function/200.ai-function.md`

  - **Description**: Comprehensive guide to AI functions including AI model management with DBMS_AI_SERVICE package, monitoring AI model usage through views, and AI function expressions (AI_COMPLETE, AI_PROMPT, AI_EMBED, AI_RERANK) with detailed syntax and examples.

## MCP Server

- **File Path**: `200.develop/400.mcp-server/400.oceanbase-mcp-server-and-ai-tool-integration-guide.md`

  - **Description**: OceanBase MCP Server guide for integrating AI tools with databases. Covers the core toolkit (execute_sql, get_ob_ash_report, vector/text/hybrid search, AI memory system tools), resource endpoints, and integration with Cursor and other MCP-compatible tools.

## Multi-Model Data

### JSON

- **File Path**: `200.develop/500.multi-model/100.json/100.json-formatted-data-types.md`

  - **Description**: JSON formatted data types in seekdb.

- **File Path**: `200.develop/500.multi-model/100.json/200.create-a-json-value.md`

  - **Description**: How to create JSON values in seekdb.

- **File Path**: `200.develop/500.multi-model/100.json/300.querying-and-modifying-json-values.md`

  - **Description**: Querying and modifying JSON values in seekdb.

- **File Path**: `200.develop/500.multi-model/100.json/400.json-formatted-data-type-conversion.md`

  - **Description**: JSON data type conversion in seekdb.

- **File Path**: `200.develop/500.multi-model/100.json/500.json-partial-update.md`

  - **Description**: JSON partial update operations in seekdb.

- **File Path**: `200.develop/500.multi-model/100.json/600.json-semi-struct.md`

  - **Description**: JSON semi-structured data handling in seekdb.

### Spatial Data

- **File Path**: `200.develop/500.multi-model/200.spatial/100.spatial-data-type-overview.md`

  - **Description**: Overview of spatial data types in seekdb for GIS applications.

- **File Path**: `200.develop/500.multi-model/200.spatial/200.spacial-reference-system.md`

  - **Description**: Spatial reference systems in seekdb.

- **File Path**: `200.develop/500.multi-model/200.spatial/300.create-spatial-columns.md`

  - **Description**: How to create spatial columns in seekdb.

- **File Path**: `200.develop/500.multi-model/200.spatial/400.create-spatial-indexes.md`

  - **Description**: How to create spatial indexes in seekdb.

- **File Path**: `200.develop/500.multi-model/200.spatial/500.spatial-data-format.md`

  - **Description**: Spatial data formats supported in seekdb.

### Character and Text

- **File Path**: `200.develop/500.multi-model/300.char-and-text/100.char-and-varchar.md`

  - **Description**: CHAR and VARCHAR data types in seekdb.

- **File Path**: `200.develop/500.multi-model/300.char-and-text/200.text.md`

  - **Description**: TEXT data type in seekdb.

- **File Path**: `200.develop/500.multi-model/300.char-and-text/300.full-text-index.md`

  - **Description**: Full-text index guide for text data in seekdb.

## SDK

### pyseekdb SDK

- **File Path**: `200.develop/900.sdk/10.pyseekdb-sdk/10.pyseekdb-sdk-get-started.md`

  - **Description**: Getting started guide for pyseekdb Python SDK. Covers installation, supported platforms (Linux embedded, macOS server mode, Windows server mode), and connection modes.

- **File Path**: `200.develop/900.sdk/10.pyseekdb-sdk/50.sdk-samples/10.pyseekdb-simple-sample.md`

  - **Description**: Simple sample for pyseekdb SDK usage.

- **File Path**: `200.develop/900.sdk/10.pyseekdb-sdk/50.sdk-samples/50.pyseekdb-complete-sample.md`

  - **Description**: Complete sample demonstrating all capabilities of pyseekdb SDK.

- **File Path**: `200.develop/900.sdk/10.pyseekdb-sdk/50.sdk-samples/100.pyseekdb-hybrid-search-sample.md`

  - **Description**: Hybrid search sample using pyseekdb SDK.

## Python Integration

- **File Path**: `200.develop/1000.python/20.using-seekdb-in-python-mode.md`

  - **Description**: Guide to using seekdb in embedded Python mode with pylibseekdb. Covers environment requirements, installation, basic operations, and SQL execution examples.

---

# Integrations

This category contains guides for integrating seekdb with various AI models, frameworks, and MCP clients.

## Model Integrations

- **File Path**: `300.integrations/100.model/100.jina.md`

  - **Description**: Guide to integrating seekdb vector search with Jina AI for multimodal search and RAG applications. Covers prerequisites, obtaining API keys, and building AI assistants.

- **File Path**: `300.integrations/100.model/200.openai.md`

  - **Description**: Guide to integrating seekdb with OpenAI API for vector storage and embedding-based search. Covers converting data to vectors using OpenAI API and storing them in seekdb.

- **File Path**: `300.integrations/100.model/300.qwen.md`

  - **Description**: Guide to integrating seekdb with Tongyi Qianwen (Qwen) API for vector storage and embedding-based search using DashScope SDK.

## Framework Integrations

- **File Path**: `300.integrations/200.frame/100.langchain.md`

  - **Description**: Guide to integrating seekdb vector search with LangChain and Qwen API for Document Question Answering (DQA) applications.

- **File Path**: `300.integrations/200.frame/200.llamaindex.md`

  - **Description**: Guide to integrating seekdb vector search with LlamaIndex and Qwen API for context-augmented generative AI applications.

- **File Path**: `300.integrations/200.frame/300.springai.md`

  - **Description**: Guide to integrating seekdb vector search with Spring AI Alibaba for Java AI application development.

- **File Path**: `300.integrations/200.frame/400.dify.md`

  - **Description**: Guide to integrating seekdb vector search with Dify LLM application development platform for building production-ready generative AI applications.

- **File Path**: `300.integrations/200.frame/500.n8n.md`

  - **Description**: Guide to integrating seekdb vector search with n8n workflow automation platform to build Chat to seekdb workflows.

## MCP Client Integrations

- **File Path**: `300.integrations/300.mcp-client/100.cursor.md`

  - **Description**: Guide to integrating OceanBase MCP Server with Cursor IDE for AI-powered database interactions and rapid application development.

- **File Path**: `300.integrations/300.mcp-client/200.cline.md`

  - **Description**: Guide to integrating OceanBase MCP Server with Cline.

- **File Path**: `300.integrations/300.mcp-client/300.continue.md`

  - **Description**: Guide to integrating OceanBase MCP Server with Continue.

- **File Path**: `300.integrations/300.mcp-client/400.trae.md`

  - **Description**: Guide to integrating OceanBase MCP Server with Trae.

---

# Guides

This category contains operational guides for deploying, managing, and maintaining seekdb.

## Deployment

- **File Path**: `400.guides/400.deploy/50.deploy-overview.md`

  - **Description**: Deployment overview covering embedded mode (library in application) and server mode (single-machine deployment) with various deployment methods including pyseekdb SDK, Python, yum install, Docker containers, and OceanBase Desktop.

- **File Path**: `400.guides/400.deploy/100.prepare-servers.md`

  - **Description**: Server preparation guide for seekdb deployment.

- **File Path**: `400.guides/400.deploy/600.python-seekdb.md`

  - **Description**: Embedded deployment mode using Python.

- **File Path**: `400.guides/400.deploy/700.server-mode/100.deploy-by-systemd.md`

  - **Description**: Deploy seekdb using yum install with systemd.

- **File Path**: `400.guides/400.deploy/700.server-mode/200.deploy-by-docker.md`

  - **Description**: Deploy seekdb in a container environment using Docker.

- **File Path**: `400.guides/400.deploy/700.server-mode/300.deploy-oceanbase-desktop.md`

  - **Description**: Deploy OceanBase Desktop application for managing seekdb.

## OBShell

- **File Path**: `400.guides/1000.obshell/100.obshell-overview.md`

  - **Description**: Overview of OceanBase Shell (obshell), a local database command-line tool for administrators and developers to manage seekdb clusters and standalone instances.

- **File Path**: `400.guides/1000.obshell/300.obshell-clients/100.agent-commands.md`

  - **Description**: OBShell agent commands reference.

- **File Path**: `400.guides/1000.obshell/300.obshell-clients/200.seekdb-commands.md`

  - **Description**: OBShell seekdb commands reference.

- **File Path**: `400.guides/1000.obshell/300.obshell-clients/300.utilities-commands.md`

  - **Description**: OBShell utilities commands reference.

- **File Path**: `400.guides/1000.obshell/900.configure-monitor.md`

  - **Description**: Guide to configuring monitoring for seekdb.

- **File Path**: `400.guides/1000.obshell/1000.error.md`

  - **Description**: OBShell error reference and troubleshooting.

## Reference

- **File Path**: `400.guides/1200.reference/1100.mysql-compatibility.md`

  - **Description**: MySQL compatibility reference for seekdb.

- **File Path**: `400.guides/1200.reference/1500.telemetry.md`

  - **Description**: Telemetry reference for seekdb.

## Release Notes

- **File Path**: `400.guides/1300.release-notes/10.v1.0.0.md`

  - **Description**: Release notes for seekdb V1.0.0 (released November 14, 2025). Covers version information, product architecture, core advantages, main features, and new capability overview.

---

# Tutorials

This category contains step-by-step tutorials for building AI applications with seekdb.

## Build AI Application Demos

- **File Path**: `500.tutorials/100.create-ai-app-demo/100.build-kb-in-seekdb.md`

  - **Description**: Tutorial for building a MineKB (personal local knowledge base) desktop application using seekdb. Covers multi-project management, document processing, intelligent search with HNSW indexes, conversational Q&A with LLMs, and local storage for privacy.

- **File Path**: `500.tutorials/100.create-ai-app-demo/300.build-multi-model-application-based-on-oceanbase.md`

  - **Description**: Tutorial for building a cultural tourism assistant using seekdb's multi-model integration. Covers combining spatial data with vector search for location-aware recommendations, hybrid GIS and vector queries, and LLM Agent workflow for travel planning.

- **File Path**: `500.tutorials/100.create-ai-app-demo/400.build-image-search-app-in-seekdb.md`

  - **Description**: Tutorial for building an image search application using seekdb's vector search technology. Covers image vectorization, storing image vectors, and performing similarity search for image-to-image retrieval.

---

# Quick Reference

## Common Topics by Use Case

### Getting Started with seekdb
- seekdb Overview: `100.get-started/10.overview/10.seekdb-overview.md`
- Quick Deploy (Docker): `100.get-started/100.client-server-mode/10.deploy-seekdb-testing-environment.md`
- Basic SQL Operations: `100.get-started/100.client-server-mode/15.basic-sql-operations.md`

### Vector Search
- Vector Search Intro: `200.develop/100.vector-search/100.vector-search-overview/100.vector-search-intro.md`
- Experience Vector Search: `100.get-started/100.client-server-mode/30.experience-vector-search.md`
- Vector Indexes: `200.develop/100.vector-search/200.vector-index/200.dense-vector-index.md`

### Full-Text Search
- Experience Full-Text Indexing: `100.get-started/100.client-server-mode/40.experience-full-text-indexing.md`
- Full-Text Index Guide: `200.develop/500.multi-model/300.char-and-text/300.full-text-index.md`

### Hybrid Search
- Experience Hybrid Search: `100.get-started/100.client-server-mode/50.experience-hybrid-search.md`
- Hybrid Search with DBMS_HYBRID_SEARCH: `200.develop/200.hybrid-search/100.vector-index-hybrid-search.md`

### AI Functions
- Experience AI Functions: `100.get-started/100.client-server-mode/60.experience-ai-function.md`
- AI Function Reference: `200.develop/300.ai-function/200.ai-function.md`

### Python SDK
- pyseekdb Getting Started: `200.develop/900.sdk/10.pyseekdb-sdk/10.pyseekdb-sdk-get-started.md`
- Embedded Python Mode: `200.develop/1000.python/20.using-seekdb-in-python-mode.md`

### MCP Integration
- OceanBase MCP Server: `200.develop/400.mcp-server/400.oceanbase-mcp-server-and-ai-tool-integration-guide.md`
- Cursor Integration: `300.integrations/300.mcp-client/100.cursor.md`
- Vibe Coding with Cursor: `100.get-started/100.client-server-mode/80.experience-vibe-coding-paradigm-with-cursor-agent-oceanbase-mcp.md`

### Framework Integrations
- LangChain: `300.integrations/200.frame/100.langchain.md`
- LlamaIndex: `300.integrations/200.frame/200.llamaindex.md`
- Dify: `300.integrations/200.frame/400.dify.md`

