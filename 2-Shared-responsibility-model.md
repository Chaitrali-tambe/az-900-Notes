## Shared Resposibility model
The IT departent is responsible for maintaining the physical space, ensuring security, and maintaining or replacing the servers if anything happens. With the shared responsibility model, these responsibilities get shared between the cloud provider and the consumer. Physical security, power, cooling, and network connectivity are the responsibility of the cloud provider.


```mermaid
	graph LR
    %% Styles and Themes
    classDef customer fill:#2c3e50,stroke:#1a252f,stroke-width:2px,color:#fff;
    classDef shared fill:#e67e22,stroke:#d35400,stroke-width:2px,color:#fff;
    classDef provider fill:#7f8c8d,stroke:#95a5a6,stroke-width:1px,color:#fff;
    classDef groupStyle fill:#f8f9fa,stroke:#bdc3c7,stroke-width:1px,stroke-dasharray: 5 5;

    %% --- MAP-STYLE INLINE LEGEND ---
    L1["🔵 Customer Retained"]:::customer --> SaaS
    L2["🟠 Shared Responsibility"]:::shared --> PaaS
    L3["⚪ Provider Managed"]:::provider --> IaS

    %% --- SAAS COLUMN ---
    subgraph SaaS [SaaS]
        S1[Information and data]:::customer
        S2[Devices mobiles & PCs]:::customer
        S3[Accounts and Identities]:::customer
        S4[Identity & directory infra]:::shared
        S5[Applications]:::provider
        S6[Network Controls]:::provider
        S7[Operating System]:::provider
        S8[Physical hosts]:::provider
        S9[Physical network]:::provider
        S10[Physical Datacenter]:::provider
    end

    %% --- PAAS COLUMN ---
    subgraph PaaS [PaaS]
        P1[Information and data]:::customer
        P2[Devices mobiles & PCs]:::customer
        P3[Accounts and Identities]:::customer
        P4[Identity & directory infra]:::shared
        P5[Applications]:::shared
        P6[Network Controls]:::shared
        P7[Operating System]:::provider
        P8[Physical hosts]:::provider
        P9[Physical network]:::provider
        P10[Physical Datacenter]:::provider
    end

    %% --- IAAS COLUMN ---
    subgraph IaS [IaaS]
        I1[Information and data]:::customer
        I2[Devices mobiles & PCs]:::customer
        I3[Accounts and Identities]:::customer
        I4[Identity & directory infra]:::customer
        I5[Applications]:::customer
        I6[Network Controls]:::customer
        I7[Operating System]:::customer
        I8[Physical hosts]:::provider
        I9[Physical network]:::provider
        I10[Physical Datacenter]:::provider
    end

    %% --- ON-PREMISE COLUMN ---
    subgraph OnPrem [On-Premise]
        O1[Information and data]:::customer
        O2[Devices mobiles & PCs]:::customer
        O3[Accounts and Identities]:::customer
        O4[Identity & directory infra]:::customer
        O5[Applications]:::customer
        O6[Network Controls]:::customer
        O7[Operating System]:::customer
        O8[Physical hosts]:::customer
        O9[Physical network]:::customer
        O10[Physical Datacenter]:::customer
    end

    %% Layout anchor for OnPrem column
    L3 --> OnPrem

    %% Apply group styles
    style SaaS groupStyle
    style PaaS groupStyle
    style IaS groupStyle
    style OnPrem groupStyle



```
