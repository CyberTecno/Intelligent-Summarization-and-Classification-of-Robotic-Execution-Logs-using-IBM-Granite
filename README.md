This project demonstrates how Large Language Models (LLMs) like IBM Granite can be applied to robotics data analytics  specifically to summarize and identify patterns within robotic execution logs.

Robotic systems generate extensive log data that is often difficult to interpret manually.
By leveraging IBM Granite's summarization and reasoning capabilities, this project transforms raw log data into structured, human-readable insights that highlight:

##  Key operational events

    1. Common failure types
    2. Root cause patterns
    3. Recommended corrective actions

The project combines Summarization (to compress log data into actionable insights) and Mini Classification (to categorize detected failure patterns).

## Technical Stack

| Technical | Tools |
|------|--------------|
| AI Model | IBM Granite 3.3-8B Instruct |
| Platform | Google Colab |
| Integration | Replicate API |
| Language | Python |
| Libraries | langchain_community, replicate, pandas, matplotlib |



## Key Features

    1. Automatic log summarization using AI
    2. Classification insight extraction for error type detection
    3. Adjustable model parameters (top_k, top_p, max_tokens, repetition_penalty)
    4. Clean visual and structured outputs
