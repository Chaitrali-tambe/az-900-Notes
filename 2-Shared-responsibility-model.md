## Shared Resposibility model
The IT departent is responsible for maintaining the physical space, ensuring security, and maintaining or replacing the servers if anything happens. With the shared responsibility model, these responsibilities get shared between the cloud provider and the consumer. Physical security, power, cooling, and network connectivity are the responsibility of the cloud provider.


```mermaid
	graph TD
    %% Styles and Themes
    classDef customer fill:#2c3e50,stroke:#1a252f,stroke-width:2px,color:#fff;
    classDef shared fill:#e67e22,stroke:#d35400,stroke-width:2px,color:#fff;
    classDef provider fill:#7f8c8d,stroke:#95a5a6,stroke-width:1px,color:#fff;
    classDef groupStyle fill:#f8f9fa,stroke:#bdc3c7,stroke-width:1px;

    %% --- INLINE LEGEND NODES (NO SUBGRAPH) ---
    L1["🟦 Customer Managed"]:::customer --> SaaS
    L2["🟧 Shared Responsibility"]:::shared --> PaaS
    L3["🟫 Provider Managed"]:::provider --> IaaS

    %% --- SAAS COLUMN ---
    subgraph SaaS [SaaS]
        direction TB
        S1[Data & Info]:::customer -->
        S2[Devices]:::customer -->
        S3[Identities]:::customer -->
        S4[Identity Infra]:::shared -->
        S5[Applications]:::provider -->
        S6[Network Ctrl]:::provider -->
        S7[OS]:::provider -->
        S8[Hosts]:::provider -->
        S9[Phys Net]:::provider -->
        S10[Datacenter]:::provider
    end

    %% --- PAAS COLUMN ---
    subgraph PaaS [PaaS]
        direction TB
        P1[Data & Info]:::customer -->
        P2[Devices]:::customer -->
        P3[Identities]:::customer -->
        P4[Identity Infra]:::shared -->
        P5[Applications]:::shared -->
        P6[Network Ctrl]:::shared -->
        P7[OS]:::provider -->
        P8[Hosts]:::provider -->
        P9[Phys Net]:::provider -->
        P10[Datacenter]:::provider
    end

    %% --- IAAS COLUMN ---
    subgraph IaaS [IaaS]
        direction TB
        I1[Data & Info]:::customer -->
        I2[Devices]:::customer -->
        I3[Identities]:::customer -->
        I4[Identity Infra]:::customer -->
        I5[Applications]:::customer -->
        I6[Network Ctrl]:::customer -->
        I7[OS]:::customer -->
        I8[Hosts]:::provider -->
        I9[Phys Net]:::provider -->
        I10[Datacenter]:::provider
    end

    %% --- ON-PREMISE COLUMN ---
    subgraph OnPrem [On-Premise]
        direction TB
        O1[Data & Info]:::customer -->
        O2[Devices]:::customer -->
        O3[Identities]:::customer -->
        O4[Identity Infra]:::customer -->
        O5[Applications]:::customer -->
        O6[Network Ctrl]:::customer -->
        O7[OS]:::customer -->
        O8[Hosts]:::customer -->
        O9[Phys Net]:::customer -->
        O10[Datacenter]:::customer
    end

    %% Additional layout alignment
    L3 --> OnPrem

    %% Apply group styles to columns
    style SaaS groupStyle
    style PaaS groupStyle
    style IaaS groupStyle
    style OnPrem groupStyle

```
