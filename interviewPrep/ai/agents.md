# Build AI Agents from scratch
  From a software engineering perspective, an agent is not an independent entity but a traditional software application that uses a language model for dynamic routing and decision‑making.
  Building reliable agents doesn’t need complex frameworks; it requires 
      solid engineering rigor, 
      state management, 
      input validation, 
      structured database queries, and 
      error handling.

  large language models into software architectures, a common engineering error is default delegation of all system routing to fully autonomous agents. 
  In production environments, full autonomy introduces variables that complicate testing, debugging, and cost control.
  
    Autonomy is not a binary choice, but a continuum known as the **Fixedness Spectrum**

  The Fixedness Spectrum is divided into three distinct design patterns, each suited to different problem profiles:
  1. Workflows (Highly Fixed)
         A workflow is a deterministic sequence of operations defined entirely in code. The application execution path is fixed.
         The language model is restricted to parsing inputs (e.g., extracting fields from a document) or generating text at predefined stages.

     Path: Step A → Step B → Step C (always constant).
     Characteristics: High predictability, low latency, low API costs, simple to test.
     Use Case: Actions with clear, unvarying business rules, such as checking order shipment details and email confirmation.
  
  2. Routers (Conditional Routing)
           A The pattern uses a classification component, often a small, fast language model or a heuristic rule engine,
           to inspect incoming text and route requests to a predefined deterministic workflow.

      Path: Input → Router → Select workflow X, Y, or Z → Execute.
      Characteristics: High predictability post-routing, low-to-moderate latency, moderate API costs.
      Use Case: Support desks sorting customer requests into distinct categories (e.g., billing disputes, technical issues, return requests).

  3. Agents (Highly Autonomous)
            An agent is given a set of tool descriptions (functions) and an open-ended goal. The language model determines the sequence of tool executions dynamically.
            At each turn, it reviews previous outputs to decide the next step, terminating only when its goal is achieved.

     Path: Input → Tool A → Observe output → Tool B → Observe output → Terminate.
     Characteristics: High flexibility, nondeterministic execution path, high latency, high API costs.
     Use Case: Complex, multi-step queries where the exact sequence of lookups depends on runtime information (e.g., investigating a damaged item delivery involving checking orders, looking up warranty policies, and deciding compensation).

The Principle of Parsimony
        
        [!IMPORTANT] The Rule of Parsimony: Use the least autonomous pattern that satisfies the system requirements.
  
  If a business task can be executed using a workflow or a simple router, implementing an agent introduces unnecessary complexity. 
  Autonomy should be reserved solely for tasks where the sequence of operations cannot be predicted before runtime.  


### The Core Loop : Bare Metal Implementation
  
  Mechanics of the Execution Loop
    Rather than delegating control flow to complex third-party abstractions, developers can implement agents using standard loops and conditional branching.

  Structural Decoupling
    Reviewing the loop implementation highlights two architectural patterns:
        Decoupling Reasoning and Action: The language model only emits a string requesting an action. It has no mechanism to execute the database query itself. The actual database execution happens strictly within the application environment. This preserves control boundaries.
        State Accumulation: The outcomes of function executions must be appended to the conversation history message list before the next turn starts. This history is what provides the stateless model with short-term context memory.
