# Platform as a Service (PaaS) in Azure 

```mermaid
graph LR
    %% Styles and Themes
    classDef customer fill:#2c3e50,stroke:#1a252f,stroke-width:2px,color:#fff;
    classDef shared fill:#e67e22,stroke:#d35400,stroke-width:2px,color:#fff;
    classDef provider fill:#7f8c8d,stroke:#95a5a6,stroke-width:1px,color:#fff;
    classDef groupStyle fill:#f8f9fa,stroke:#bdc3c7,stroke-width:1px,stroke-dasharray: 5 5;

    %% --- MAP-STYLE INLINE LEGEND ---
    L1["🔵 Customer Managed"]:::customer --> PaaS
    L2["🟠 Shared Responsibility"]:::shared --> PaaS
    L3["⚪ Provider Managed"]:::provider --> PaaS

    %% --- PAAS ONLY COLUMN (CONNECTED LANDSCAPE) ---
    subgraph PaaS [Platform as a Service - PaaS]
        direction LR
        I1[Information and data]:::customer -->
        I2[Devices mobiles & PCs]:::customer -->
        I3[Accounts and Identities]:::customer -->
        I4[Identity & directory infra]:::shared -->
        I5[Applications]:::shared -->
        I6[Network Controls]:::shared -->
        I7[Operating System]:::provider -->
        I8[Physical hosts]:::provider -->
        I9[Physical network:::provider -->
        I10[Physical Datacenter]:::provider
    end

    %% Apply group style
    style PaaS groupStyle

```


PaaS provides a framework for developers to build, test, and deploy applications without worrying about underlying infrastructure management.

### How it Works: 
Azure handles the OS, middleware, and runtime. You focus solely on developing and managing your application code and data.

### Azure Examples: 
Azure App Service, Azure SQL Database, Azure Functions, Azure Kubernetes Service (AKS).

### Pros: 
<dl>
    <dd> ► <strong>Faster Development:</strong> Accelerates development cycles by removing infrastructure setup.</dd>
    <dd> ► <strong>Reduced Maintenance:</strong> Azure handles patching and OS updates.</dd>
    <dd> ► <strong>Cost-Effective:</strong> Pay only for resources consumed, reducing idle hardware costs.</dd>
</dl>

### Cons:
<dl>
    <dd> ► <strong>Limited Customization:</strong> Less control over the underlying infrastructure and configuration.</dd>
    <dd> ► <strong>Vendor Lock-in:</strong> Applications may be tied specifically to Azure services. </dd>
</dl>
