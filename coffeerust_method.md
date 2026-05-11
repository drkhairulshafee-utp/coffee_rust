---
config:
  layout: fixed
---
flowchart TB
 subgraph Phase1["1. Preliminary Investigation"]
        B["Stakeholder Needs"]
        A["Literature Review"]
        C["Technical Benchmarking"]
  end
 subgraph Phase2["2. Dataset & AI Training"]
        E["Preprocessing & Augmentation"]
        D["Data Sourcing"]
        F["CNN Model Training"]
        G["Performance Evaluation"]
  end
 subgraph Phase3["3. AR Development"]
        I["Real-time Inference Logic"]
        H["AR SDK Integration"]
        J["UI/UX Design"]
  end
 subgraph Phase4["4. Integration & Validation"]
        K["System Integration"]
        L["Functional Testing"]
        M["Early Identification & Treatment Output"]
  end
    A --> B
    B --> C
    D --> E
    E --> F
    F --> G
    H --> I
    I --> J
    K --> L
    L --> M
    Phase2 --> Phase4
    Phase3 --> Phase4
    Phase1 --> Phase2
