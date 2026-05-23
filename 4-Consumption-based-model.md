# Consumption-based model 

```mermaid
graph LR
    %% Main Connections
    A([Consumption-based model]) --- B(Capex)
    A --- C(Opex)

    %% Connections
    B --- B1[Resource]
    C --- B1
    B1 --- B2(Buy)
    B2 --- B3(Use)
    B1 --- C1(Scale)
    C1 --- C2(Pay)

    %% Main Cloud Models (Light Blue)
    style B fill:#d0e1fd,stroke:#4a90e2,stroke-width:2px,color:#000
    style C fill:#d0e1fd,stroke:#4a90e2,stroke-width:2px,color:#000

    %% Shared Node (Light Pink)
    style B fill:#d0e1fd,stroke:#ffc0cb,stroke-width:2px,color:#000
    
    %% Example Bubbles (Light Gray)
    style B1 fill:#f0f0f0,stroke:#999,stroke-width:1px,color:#333
    style B2 fill:#f0f0f0,stroke:#999,stroke-width:1px,color:#333
    style C1 fill:#f0f0f0,stroke:#999,stroke-width:1px,color:#333
    style C2 fill:#f0f0f0,stroke:#999,stroke-width:1px,color:#333
```

### Capex: 
Buy resource and then use. Paying for all the resources you are buying, whether you may use it or not.

### Opex:
Scaling resource as per need and paying for it based on usage like a bill.

## Cloud computing uses Opex.
This consumption-based model has many benefits, including:
<dl>
   <dd>▪ No upfront costs. </dd>
   <dd>▪ No need to purchase and manage costly infrastructure that users might not use to its fullest potential. </dd>
   <dd>▪ The ability to pay for more resources when they're needed. </dd>  
   <dd>▪ The ability to stop paying for resources that are no longer needed. </dd>
</dl>

