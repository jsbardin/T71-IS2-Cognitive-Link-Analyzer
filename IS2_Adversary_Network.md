# Cognitive Network Link Analysis

Copy the code block below into a Mermaid Live Editor or compatible Markdown viewer. The structure maps an adversary disinformation network from state-sponsor down to local proxies.

```mermaid
graph TD
    A[State Intelligence Apparatus] -->|Directs Funding| B(Front Organization)
    A -->|Provides Doctrine| C(Cyber PSYOPS Unit)
    B -->|Launders Capital| D{Local Proxy Group}
    C -->|Generates Synthetic Media| E[Social Amplification Botnet]
    C -->|Executes Stylometric Mimicry| F[Compromised Influencer]
    D -->|Organizes Physical Protests| G((Target Population))
    E -->|Saturates Information Space| G
    F -->|Establishes False Trust| G
    
    classDef state fill:#b30000,stroke:#333,stroke-width:2px,color:#fff;
    classDef proxy fill:#f9a03f,stroke:#333,stroke-width:2px;
    classDef target fill:#005c99,stroke:#333,stroke-width:2px,color:#fff;
    
    class A,C state;
    class B,D,E,F proxy;
    class G target;
