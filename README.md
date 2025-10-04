# RAG-Based Indian Government Schemes Assistant
A fully-coded Retrieval-Augmented Generation (RAG) system that delivers accurate, structured information on Indian government schemes, supporting direct queries and personalized recommendations, with LLM-based evaluation.


## Project Overview
This is the new full-code version of the Indian Government Schemes Assistant, building upon the earlier version [[link to earlier repo](https://github.com/Misty033/Government-Scheme-retrival-system-using-LLMs)] which used no-code tools.

### Earlier Version Highlights:
- Leveraged Jina AI for JSON conversion of scraped scheme data
- Scraping of government scheme information
- Orchestration using LangChain + n8n workflows
- Primarily a no-code and low-code setup

### New Version Highlights:
- Fully-coded Python implementation.
- RAG pipeline built with LangChain and vector retrieval.
- LLM-driven structured responses and step-by-step user profiling.
- LLM-based judge to evaluate responses with completeness and confidence scores.
- Interactive chat interface with memory for follow-up questions.
- No reliance on no-code tools — complete control over the pipeline.



### Key Features
- Direct Scheme Queries: Ask about eligibility, benefits, application process, documents, duration, and more.
- Suggestions: Collect user profile step-by-step and suggest schemes (Mode A).
- Structured Responses: Includes all key fields, source citations, completeness, and confidence scores.
- LLM Judge: Evaluates quality and reliability of answers.
- Memory-Enabled Conversation: Maintains context for follow-up queries.
- Full-Code Flexibility: Easier to modify, extend, or integrate with other systems.


### Technologies Used
- Python
- LangChain for RAG orchestration
- Large Language Models: Qwen2.5:8b (RAG), llama3.1:8b (Judge)
- Vector Database: ChromaDB for document retrieval
- Recursive Chunking Strategy for efficient long-document processing
- Ollama SDK for LLM calls
- ConversationBufferMemory for chat context



### How to Use

1. **Clone the repository**
```bash
git clone <this-repo-url>
```
2. **Install dependencies**
```bash
pip install -r requirements.txt
```
3. **Run the notebook: main.ipynb**
- Load preprocessed scheme documents and vector store.
- Initialize RAG chain and judge LLM chain.
- Run interactive chat for either:
  - Mode 1: Personalized scheme recommendations.
  - Mode 2: Direct scheme query.
4. **Output**
   Structured scheme information with sources, completeness, and confidence scores.



### Evaluation
- Completeness Score: Measures how many key fields are correctly filled.
- Confidence Score: Measures reliability and relevance based on retrieved sources.
- Reasoning: Brief explanation from the judge LLM.


### Future Scope
- Recommendation Engine: Suggest schemes based on user profile and preferences.
- Recommendation Evaluation: Implement proper evaluation metrics for recommendations.
- Data Updates: Automate scraping and updating of scheme information.
- Multilingual Support: Serve users in regional languages.
- Voice Assistant: Enable voice-based interaction for enhanced accessibility.

# Fully-coded approach provides more control, reliability, and extendibility compared to the no-code version.

# Related Resources
Earlier Version (No-Code / Low-Code): [Link to earlier repo](https://github.com/Misty033/Government-Scheme-retrival-system-using-LLMs)
