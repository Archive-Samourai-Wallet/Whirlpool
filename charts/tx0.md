sequenceDiagram
    autonumber

    Note over Client,Coordinator: << REST >>

    Note left of Client: Preview TX0...
    Client->>+Coordinator: POST /rest/tx0 [Tx0DataRequestV2]
    Coordinator-->>-Client: Tx0DataResponseV2

    Note left of Client: Push TX0...
    Client-->>+Coordinator: POST /rest/tx0/push [Tx0PushRequest]
    alt success
        Coordinator-->>-Client: PushTxResponse
    else error
        Coordinator-->>Client: PushTxErrorResponse
    end
