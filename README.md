# Festiva_Planner_AI
An AI-powered multi-agent event planning system that automates event organization using Machine Learning, NLP, RAG (Retrieval-Augmented Generation), and intelligent agent orchestration.

# Project Overview
Festiva Planner AI helps users plan events such as:

* Weddings
* Corporate Events
* Birthday Parties

The system can:

- Generate complete event plans
- Predict budget allocation using ML
- Retrieve planning knowledge using RAG
- Use multiple AI agents for orchestration
- Provide event timelines and recommendations

# Features
1. AI Event Planner

Generates:

* Event timeline
* Task checklist
* Budget breakdown
* Vendor category suggestions
  
Example Input

Wedding in Bangalore with budget ₹10,00,000

Example Output

Venue: ₹3,00,000
Catering: ₹2,50,000
Decoration: ₹1,50,000
Photography: ₹1,00,000
Entertainment: ₹2,00,000

2. Budget Optimization using Machine Learning
Uses:

* Random Forest Regressor
* Multi-output regression

Predicts:

* Venue cost
* Catering cost
* Decoration cost
* Photography cost
* Entertainment cost

3. RAG-Based Knowledge Assistant
Uses:

* FAISS Vector Database
* Sentence Transformers
* Semantic Search

Answers queries like:

* “How to plan a wedding?”
* “Best corporate event strategy?”
* “Birthday planning checklist”

4. Multi-Agent AI System

Planner Agent
Controls workflow and generates final event plan.

Budget Agent
Predicts optimized budget allocation.

Research Agent
Retrieves relevant planning knowledge

# Project Architecture
<img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/6c6a2b77-ce1a-4308-abc7-5b41fd207d72" />



# Project Structure
<img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/b83a46ac-e4b7-44d7-8b88-e6c7a7bf47ef" />



# Technologies Used
Programming Language
* Python
Machine Learning
* Scikit-learn
* Random Forest Regression
NLP & RAG
* LangChain
* Sentence Transformers
* HuggingFace Embeddings
Vector Database
* FAISS
Backend
* FastAPI
Deployment
* Docker
* Google Colab

# Machine Learning Workflow
Input Features
* Event Type
* Guest Count
* Total Budget
Predicted Outputs
* Venue Cost
* Catering Cost
* Decoration Cost
* Photography Cost
* Entertainment Cost

# RAG Workflow
Step 1
Load event planning documents.

Step 2
Convert text into embeddings.

Step 3
Store embeddings inside FAISS vector database.

Step 4
Retrieve relevant information using semantic similarity.


# Example API Input
{
  "event_type": "Wedding",
  "city": "Bangalore",
  "budget": 1000000,
  "guests": 300
}

# Example Output
{
  "event_type": "Wedding",
  "city": "Bangalore",
  "budget_breakdown": {
    "venue": 300000,
    "catering": 250000,
    "decoration": 150000,
    "photography": 100000,
    "entertainment": 200000
  },
  "timeline": [
    "6 Months Before → Book venue",
    "5 Months Before → Hire caterers",
    "3 Months Before → Confirm decorations"
  ]
}


# Key Concepts Used

Machine Learning
Model learns budget allocation patterns from historical event data.

NLP
Processes event-related text and user queries.

RAG (Retrieval-Augmented Generation)
Retrieves event knowledge and provides intelligent responses.

Embeddings
Converts text into numerical vectors for semantic understanding.

FAISS
Performs efficient similarity search on embeddings.

Multi-Agent Systems
Different AI agents collaborate to complete planning tasks.

# Future Improvements
* GPT-powered dynamic timeline generation
* Vendor recommendation system
* Streamlit frontend
* WhatsApp reminders
* Voice assistant
* Real-time booking APIs
* Reinforcement learning optimization
* CrewAI / LangGraph integration
  
# Learning Outcomes

This project demonstrates:

- Machine Learning
- NLP & RAG Systems
- Vector Databases
- Multi-Agent AI
- FastAPI Backend Development
- Real-world AI Architecture

# Use Cases
* Smart wedding planning
* Corporate event management
* Birthday event organization
* AI scheduling assistants
* Vendor budget optimization
