sequenceDiagram
    autonumber
    Note over Client,Soroban: << JSON-RPC >>

    Note left of Client: Registering input...
    Client->>Soroban: directory.Add: com.samourai.whirlpool.wo.inputs.<poolId> [RegisterInputSorobanMessage]
    
    Note left of Client: Waiting for a mix...
    Soroban->>Client: directory.List: <responseKey> [InviteMixSorobanMessage]
    
    Note over Client,Soroban: ... Wait for being invited to mix
