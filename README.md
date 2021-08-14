Basic Project Sample Example
This example demos a basic host application loading from different remote component.

Wrapper is the host application, which renders as container for Page1 and Page2 as well as consumes Domain and UI Components.
UIComponents standalone application which exposes baisc UI Button component.
DomainComponents standalone application which exposes enhanced UI Button component.
Page1 standalone application which exposes Page1 module built using shared remote UIComponents and DomainComponents.
Page2 standalone application which exposes Page2 module built using shared remote UIComponents and DomainComponents.
LibApp holds all the node_modules, store and context used across the remote

Running Demo
Run npm run cleanInit. This will install node_modules for LibApp, DomainComponents, UIComponents, Page1, Page2 and Wrapper.
Run npm start. This will build and serve LibApp, DomainComponents, UIComponents, Page1, Page2 and Wrapper on ports 8087, 8082, 8083, 8084, 8085 and 8086 respectively.

localhost:8085 (STANDALONE REMOTE LibApp holds all lib, store and context)
localhost:8082 (STANDALONE REMOTE DomainComponents)
localhost:8083 (STANDALONE REMOTE UIComponents)
localhost:8084 (STANDALONE REMOTE Page1)
localhost:8085 (STANDALONE REMOTE Page2)
localhost:8086 (HOST Wrapper act as a shell)
