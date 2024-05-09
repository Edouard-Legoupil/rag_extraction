# rag_extraction: Summarizing Evidence from Public Evaluation Reports

Retrieval-Augmented Generation (RAG) is an architecture that enhances the capabilities of a Large Language Model (LLM), by incorporating an information retrieval system. This system retrieves relevant data from external sources, here an evaluation report to ground the LLM’s responses. 

## How RAG Works?

 - __Generative AI Model__: The LLM generates responses based on the input prompt.

 - __Information Retrieval System__: RAG adds an information retrieval component. When given a user query, it retrieves relevant information from external data sources.

 - __Response Formulation__: The top-ranked search results from the retrieval system are used as input to the LLM. The LLM then generates a response based on both the prompt and the retrieved information.

## Benefits 

 - __Accuracy__: By incorporating external facts, RAG improves the accuracy of generative AI models. It ensures that responses are grounded in real-world information.

 - __Relevance__: RAG allows the model to provide contextually relevant answers by pulling in data from relevant sources.

 - __Trustworthiness__: Users can trust the responses more when they are backed by factual evidence.

 - __Customization__: RAG can be constrained to use content from vectorized documents, images, and other data formats specific to the organization.

 - __Control__: Organizations have control over the grounding data used by the LLM, ensuring alignment with their content and requirements.

## Steps

 - __Index the Report__: Use embedding model to index the report’s content.

 - __User Query__: When a user asks about specific aspects of the report, send their query to the retrieval system.

 - __Retrieve Relevant Sections__: The retrieval system fetches relevant sections from the report.

 - __Generate Summary__: The LLM combines the retrieved information with its own reasoning to generate a concise summary.
 

In summary, RAG bridges the gap between generative AI and factual information, making it a powerful tool for creating context-aware and trustworthy responses.
