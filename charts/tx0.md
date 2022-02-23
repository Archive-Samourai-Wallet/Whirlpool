sequenceDiagram
    autonumber

    Note over Client,Server: << REST >>
    Client->>+Server: POST /rest/tx0 [Tx0DataRequestV2]
    Server-->>-Client: Tx0DataResponseV2
    Client-->>+Wallet backend: BROADCAST tx0
