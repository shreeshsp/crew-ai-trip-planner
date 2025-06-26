# AI Crew for Trip Planning
## Introduction
This project is an example using the CrewAI framework to automate the process of planning a trip. CrewAI orchestrates autonomous AI agents, enabling them to collaborate and execute complex tasks efficiently.


## CrewAI Framework
CrewAI is designed to facilitate the collaboration of role-playing AI agents. In this example, these agents work together to choose between different of cities and put together a full itinerary for the trip based on your preferences.

## Running the Script
It uses GPT-4 by default so you should have access to that to run it.

***Disclaimer:** This will use gpt-4 unless you changed it 
not to, and by doing so it will cost you money.*

- **Configure Environment**: Copy ``.env.example` and set up the environment variables for [Serper](https://serper.dev/) and [OpenAI](https://platform.openai.com/api-keys)
- **Install Dependencies**: Run `poetry install --no-root`.
- **Execute the Script**: Run `poetry run python main.py` and input your idea.

## Details & Explanation
- **Running the Script**: Execute `python main.py`` and input your idea when prompted. The script will leverage the CrewAI framework to process the idea and generate a landing page.
- **Key Components**:
  - `./main.py`: Main script file.
  - `./tasks.py`: Main file with the tasks prompts.
  - `./agents.py`: Main file with the agents creation.
  - `./tools`: Contains tool classes used by the agents.

## Using GPT 3.5
CrewAI allow you to pass an llm argument to the agent constructor, that will be it's brain, so changing the agent to use GPT-3.5 instead of GPT-4 is as simple as passing that argument on the agent you want to use that LLM (in `main.py`).
