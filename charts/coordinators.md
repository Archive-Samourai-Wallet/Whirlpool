sequenceDiagram
    autonumber

    Note over Client,Soroban: << JSON-RPC >>
    Client->>+Soroban: directory.List: com.samourai.whirlpool.ro.coordinators

    Soroban-->>-Client: List<RegisterCoordinatorSorobanMessage>
