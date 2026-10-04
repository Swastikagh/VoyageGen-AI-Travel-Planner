# VoyageGen — AI Travel Planner

VoyageGen is an AI-powered travel planning application that generates personalized, structured travel itineraries based on user preferences. It uses **LLaMA-3 70B**, **LangChain**, and **LangGraph** to transform travel requirements into practical day-wise trip plans through an interactive **Gradio** interface.

## Features

* Personalized AI-generated travel itineraries
* Destination-based trip planning
* Day-wise itinerary generation
* User-focused travel recommendations
* Conversational AI-based planning
* LangGraph-based workflow orchestration
* Interactive Gradio web interface
* Powered by Groq's high-speed LLaMA-3 70B inference

## Tech Stack

* **Language:** Python
* **LLM:** LLaMA-3 70B
* **LLM Platform:** Groq
* **GenAI Framework:** LangChain
* **Agent/Workflow Framework:** LangGraph
* **UI:** Gradio
* **Environment:** Google Colab

## How It Works

VoyageGen follows an AI-driven workflow to convert a user's travel preferences into a structured itinerary.

```text
User Input
    ↓
Travel Preferences
    ↓
LangGraph StateGraph
    ↓
LangChain Processing
    ↓
LLaMA-3 70B via Groq
    ↓
Itinerary Generation
    ↓
Personalized Day-wise Travel Plan
    ↓
Gradio Interface
```

## Workflow

1. **User Input**

   * Destination
   * Number of days
   * Travel preferences
   * Interests and requirements

2. **State Management**

   * LangGraph `StateGraph` manages the travel-planning workflow and maintains the required state throughout the generation process.

3. **AI Processing**

   * LangChain handles the LLM interaction and prompt-based processing.
   * LLaMA-3 70B generates travel recommendations and itinerary content through Groq.

4. **Itinerary Generation**

   * The system organizes the generated information into a structured travel plan.

5. **Interactive Output**

   * Gradio provides a simple interface for users to enter their requirements and view the generated itinerary.

## Example Use Case

A user can provide:

```text
Destination: Manali
Duration: 4 Days
Interests: Nature, Adventure, Local Food
Budget: Moderate
```

VoyageGen generates a personalized itinerary with activities and recommendations organized across the trip.

## Project Structure

```text
VoyageGen/
│
├── VoyageGen.ipynb
├── README.md
└── requirements.txt
```

## Installation

Clone the repository:

```bash
git clone https://github.com/Swastikagh/VoyageGen.git
cd VoyageGen
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

## API Configuration

VoyageGen uses Groq for LLaMA-3 inference.

Create a Groq API key and configure it in your environment:

```python
import os

os.environ["GROQ_API_KEY"] = "your_api_key"
```

For security, do not commit API keys directly to GitHub.

## Running the Project

The project can be executed directly through Google Colab or as a Python application after installing the required dependencies.

Run the Gradio interface and interact with the AI travel planner through the generated interface.

## Key Technologies

### LangChain

Used to connect the application with the LLM and manage prompt-based AI interactions.

### LangGraph

Used to build and manage the travel-planning workflow using a state-based graph architecture.

### LLaMA-3 70B

Acts as the core language model responsible for understanding travel requirements and generating itinerary recommendations.

### Groq

Provides high-speed inference for the LLaMA-3 model.

### Gradio

Provides the interactive user interface for the travel planning application.

## Future Improvements

* Real-time flight and hotel integration
* Live weather information
* Maps and route optimization
* Budget estimation and expense tracking
* Restaurant recommendations
* Multi-destination trip planning
* Tool-calling and external API integration
* Persistent user preferences
* Deployment as a production web application

## Learning Outcomes

Through this project, I explored:

* Generative AI application development
* LLM integration using Groq
* LangChain
* LangGraph and state-based workflows
* Prompt engineering
* AI-powered recommendation systems
* Interactive GenAI interfaces using Gradio

## Author

**Swastika Chakraborty**

B.Tech CSE | AI/ML & Generative AI

GitHub: **Swastikagh**
