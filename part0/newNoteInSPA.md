```mermaid
sequenceDiagram
participant browser
participant server

    Note over browser: JS executes and parses JSON data

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: JSON data added to list in DOM
    deactivate server
```
