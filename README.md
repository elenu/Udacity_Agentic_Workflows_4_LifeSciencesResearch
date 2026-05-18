# Final Project Course of Agentic Workflows for Life Sciences Research

Main aim of this project focused in developing a drug repositioning agentic workflow.

I implemented a multi-agent system that automates drug repurposing investigations by 
leveraging specialized AI agents to plan workflows, route tasks, mine biomedical databases
for potential drug candidates, enrich these candidates with literature and safety data, 
and ultimately score, rank, and create a validation roadmap through an evaluator-optimizer 
loop. You can find the corresponding code inside ```starter/scaffold.py```.

## Demonstrated Learning Objectives

Objectives I achieved with this project:
- Sequential workflows (DataMiningAgent)
- Prompt chaining (LiteratureAgent: search -> assess)
- LLM-based routing (RoutingAgent)
- Evaluator-optimizer pattern (EvaluationAgent)
- Multi-agent orchestration (DrugRepurposingOrchestrator)

## How to run it

Mock mode (no API keys needed, used for development):
```USE_MOCK_DATA=true``` <- In ```env.txt``` (you need to save as .env)
```python scaffold.py```

Live mode (requires API keys):
```OPENAI_API_KEY=your_key``` <- In ```env.txt``` (you need to save as .env)
```python scaffold.py```
