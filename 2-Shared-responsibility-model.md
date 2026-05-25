## Shared Resposibility model
The IT departent is responsible for maintaining the physical space, ensuring security, and maintaining or replacing the servers if anything happens. With the shared responsibility model, these responsibilities get shared between the cloud provider and the consumer. Physical security, power, cooling, and network connectivity are the responsibility of the cloud provider.


```mermaid
	%%{init: {'flowchart': {'rankSpacing': 10, 'nodeSpacing': 5}, 'themeVariables': {'nodePadding': 4, 'fontSize': '12px'}}}%%
graph TD
    %% Styles and Themes
    classDef customer fill:#2c3e50,stroke:#1a252f,stroke-width:1px,color:#fff;
    classDef provider fill:#7f8c8d,stroke:#95a5a6,stroke-width:1px,color:#fff;
    classDef groupStyle fill:#f8f9fa,stroke:#bdc3c7,stroke-width:1px;

    %% --- INLINE LEGEND NODES ---
    L1["🟦 Customer Managed (◼)"]:::customer --- IaaS
    L2["🟫 Provider Managed (☐)"]:::provider --- IaaS

    %% --- COMPACT IAAS COLUMN ---
    subgraph IaaS [IaaS]
        direction TB
        I1[Information and data ◼]:::customer ---
        I2[Devices mobiles & PCs ◼]:::customer ---
        I3[Accounts and Identities ◼]:::customer ---
        I4[Identity & directory infra ◼]:::customer ---
        I5[Applications ◼]:::customer ---
        I6[Network Controls ◼]:::customer ---
        I7[Operating System ◼]:::customer ---
        I8[Physical hosts ☐]:::provider ---
        I9[Physical network ☐]:::provider ---
        I10[Physical Datacenter ☐]:::provider
    end

    %% Apply group style
    style IaaS groupStyle


```
