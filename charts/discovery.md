classDiagram

class Samourai {
-signingAddress [permanent identity]
}

class Coordinator{
- sender [permanent identity]
- auth [signed by Samourai]
}

class Client{
-sender [temporary identity]
}

    Samourai "authenticates" --> Coordinator
    Coordinator "registers" --> Soroban
    Client "discovers coordinators" --> Soroban
    