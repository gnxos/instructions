
## Hugging Face vs PyTorch 
### Hugging Face : Library of pretrained models - collabrative hub for AI developers
    - started as a chatbot company, turned into Github of machine learning
    - Helps develop, deploy and train ML models 
    - offers infrastructure to demonstrate, operate, and integrate AI into real-world applications
  Features :
    - Transformers library with pretrained models 
    - Focus on NLP applications
    - Growing community and ecosystem

### PyTorch : Powerful deep learning framework, used for building custom NLP models from scratch. 
    - offers library pre-configured and pre-trained models 
    - Supports various neural network architectures 
    - Combines Torch's ML library with a Python-based high-level APIs
  Features :
    - Dynamic computation graph - allowes network architecture changes on the fly during runtime.

### Using Pre-Trained Transformers and Fine Tuning 
    
    BERT, Llama and GPT 

  Fine tuning LLMs adapt pre-trained models to specific tasks or domains with domain specific data. This process adjusts the models parameters to improve task performance leveraging pre-existing language understanding. 
  Fine tuning enhances efficiency and saves time and computational resources compared to training models from scratch

  Benifits of Fine-Tuning 
    Transfer Learning 

  Pitfalls of Fine-Tuning
    - Overfitting - Avoid using a small dataset or extending training epochs excessively
    - Underfitting - Ensure sufficient training and an appropriate learning rate to enable adequate learning
    - Catastrophic forgetting - Prevent the model from losing its initial broad knowledge
    - Data leakage - Keep training and validation datasets separate 

Types of Fine-tuning 
  - Self-supervised fine tuning 
  - Supervised fine tuning 
  - RLHF : Reinforcement learning from human feedback

Direct Preference Optimization (DPO) : Optimizes language models directly based on human preferences.
        - Simplicity : 
        - Human centric optimization
        - No reward training 
        - Faster convergence 

Supervised Fine-tuning 
        - Full Fine-Tuning : All parameters are tuned for the specific task
        - Parameter-Efficient Fine-Tuning (PEFT) : Fine-tuning without modifying most of the original parameters. 

