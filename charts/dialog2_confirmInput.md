sequenceDiagram
    autonumber
    Note over Client,Server: << WEBSOCKET >>

    Note left of Client: Connecting...
    Client-->>+Server: connect /ws/connect
    Client->>+Server: subscribe /private/reply (header: $poolId)
    Server-->>Client: ConfirmInputMixStatusNotification

    Note left of Client: Trying to join a mix...
    Client ->>+Server: /ws/confirmInput [ConfirmInputRequest]
    Server -->>-Client: ConfirmInputResponse
    Note left of Client: Joined a mix!

    Note over Client,Server: ... Wait for enough peers
