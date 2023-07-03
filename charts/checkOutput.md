sequenceDiagram
    autonumber

    Note over Client / alt. identity,Coordinator: << REST >> from alternate identity
    Client / alt. identity->>+Coordinator: POST /rest/checkOutput [CheckOutputRequest]

    Coordinator->>-Client / alt. identity: [HTTP SUCCESS 200]
