# Multi-Agent Customer Outreach with CrewAI

This project demonstrates a **multi-agent customer outreach workflow** built with **CrewAI**, where AI agents collaborate to analyze a lead and generate a personalized outreach campaign.

The notebook also showcases the use of **tools** in CrewAI, including built-in tools and a custom tool.

## Overview

This project simulates a sales and outreach workflow with two specialized agents:

- **Sales Representative** – researches and profiles a potential lead
- **Lead Sales Representative** – uses the profiling insights to create a personalized outreach campaign

The system is designed to show how agent collaboration can support lead generation, customer research, and personalized communication.

## Key Concepts Demonstrated

This notebook focuses on:

- **Multi-agent collaboration**
- **Sequential task execution**
- **Tool usage in CrewAI**
- **Custom tool creation**
- **Lead analysis and outreach generation**

## Agents

### 1. Sales Representative
Responsible for identifying and analyzing high-value leads based on the provided company and industry information.

### 2. Lead Sales Representative
Uses the lead profiling report to craft a targeted and personalized outreach message for a decision-maker.

## Tools Used

The notebook demonstrates both built-in and custom tools:

- **DirectoryReadTool** – reads files from a directory
- **FileReadTool** – reads file contents
- **SerperDevTool** – performs web search for additional information
- **SentimentAnalysisTool** – custom CrewAI tool used to analyze tone and support engaging outreach content

## Workflow

The workflow follows these steps:

1. Research and profile the lead
2. Gather relevant company insights
3. Pass the profiling output to the next task
4. Generate a personalized outreach campaign

This shows how agents can work together in a structured pipeline.

## Technologies Used

- Python
- CrewAI
- crewai_tools
- LangChain Community
- OpenAI GPT models
- Jupyter Notebook

## File

- `L4_tools_customer_outreach.ipynb` – main notebook for the customer outreach workflow

## Installation

Install the required libraries:

```bash
pip install crewai==0.28.8 crewai_tools==0.1.6 langchain_community==0.0.29
````

You may also need:

* OpenAI API key
* Serper API key

## How to Run

1. Open the notebook:
   `L4_tools_customer_outreach.ipynb`
2. Set your API keys
3. Run the cells in order
4. Provide the input lead information
5. Execute the crew workflow
6. Review the generated profiling report and outreach campaign

## Example Input

The notebook includes an example using:

* **Lead name:** DeepLearningAI
* **Industry:** Online Learning Platform
* **Decision-maker:** Andrew Ng
* **Position:** CEO
* **Milestone:** Product launch

## Learning Objectives

This project is useful for understanding:

* how CrewAI agents collaborate on business tasks
* how task outputs flow between agents
* how tools improve agent capabilities
* how to create and use custom tools in CrewAI

## Future Improvements

Possible extensions include:

* adding CRM integration
* exporting outreach emails automatically
* using real sentiment analysis models
* adding retrieval over internal lead documents
* deploying as a web application

## Notes

* Outputs can vary across runs because LLMs are non-deterministic
* This project is mainly educational and demonstrates the foundations of tool-augmented multi-agent outreach
* The current design uses a sequential workflow

## License

For educational and demonstration purposes.

```
