

### Introduction to LangChain 
  An open source framework that simplifies application development process to Integrate Language Models.
  Components 
    - Documents
    - Chains
    - Agents
    - Language Model
    - Chat model
    - Chat message
    - Prompt templates
        - String Prompt template
        - Chat Prompt template
        - Message Prompt template
            - AI Message Prompt template
            - System Message Prompt template
            - Human Message Prompt template
            - Chat Message Prompt template
        - Message Placeholder
        - Few Shot Prompt Template
    - Output parsers
  
#### Prompting
1. Zero shot prompt : 
    Gives the LLM a single example to help it perform a similar task.
   
3. Few shot prompt : 
    Learns from a small set of examples before tackling a similar task to generalize from a few instances to new data.
   
4. Chain-of-thought (COT) prompting : 
    Guides LLMs through complex reasoning in a step-by-step manner. Effective where the solution requires multiple intermediate steps or reasoning that mimics human thought processes.

Self consistency: 
    Used to enhance the reliability and accuracy of outputs
    Generates multiple independent answers to the same question
    Evaluates these to determine the most consistent result

