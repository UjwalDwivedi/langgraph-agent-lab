LangGraph Agent Laboratory

This repository contains a collection of Jupyter Notebooks demonstrating various advanced LLM agent workflows. It serves as a practical implementation of stateful, multi-actor applications, exploring different graph-based routing techniques and prompt chaining strategies using LangGraph and the Google Gemini API.

Implemented Workflows

Rather than standard linear scripts, this repository focuses on graph-based architectural patterns for AI agents. The key workflow concepts introduced include:
Conditional Routing: Implementing decision-making nodes within a StateGraph to evaluate conditions (such as user sentiment or error states) and dynamically route the execution flow to the appropriate subsequent nodes using conditional edges.

Prompt Chaining: Designing sequential pipelines where the structured output of one LLM directly informs and constructs the prompt for the next step, ensuring highly focused and context-aware generations.

Structured State Management: Utilizing TypedDict and Pydantic models to strictly define, maintain, and pass state variables (both text and numeric) across multiple execution nodes without data loss.

Domain-Specific Logic: Applying these graph-based patterns to targeted use cases, including mathematical problem-solving, structured essay evaluation, and state-based calculations.

Technology Stack

Frameworks: LangGraph, LangChain

Models: Google Gemini 2.5 Flash (via langchain-google-genai)

State Management: TypedDict, Pydantic (BaseModel)

Environment: Python 3.12, Jupyter Notebooks

Local Setup and Installation

Follow these steps to run the workflows on your local machine.

1. Clone the repository
git clone https://github.com/UjwalDwivedi/langgraph-agent-lab.git
cd langgraph-agent-lab

2. Configure the virtual environment
python3 -m venv .venv
source .venv/bin/activate

3.Install dependencies
pip install langgraph langchain-google-genai python-dotenv pydantic jupyter

4. Configure Environment Variables
Create a .env file in the root directory to store your API keys. This file is ignored by Git to maintain security.

5. Execute the Notebooks
Launch your preferred Jupyter environment (such as VS Code or Jupyter Lab), ensure the .venv kernel is selected, and execute the cells within the notebooks.

