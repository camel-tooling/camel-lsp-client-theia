# Camel LSP Client for Eclipse Theia

The support of Camel LSP for Eclipse Theia is in progress. It will allow to have it also with Che 7.

The idea is to rely on [Camel VS Code extension](https://marketplace.visualstudio.com/items?itemName=camel-tooling.vscode-apache-camel).

## How to install client in Theia for test purpose

### a non published Camel VS Code extension

Follow instructions [here](https://github.com/theia-ide/theia/wiki/Testing-VS-Code-extensions)

### a published Camel VS Code extension

In this case, it might be more straightforward to use the "Deploy plugin by ID" command with a Dockerized Theia.

Start theia-full as indicated [here](https://github.com/theia-ide/theia-apps#theia-docker):

docker run -it -p 3000:3000 -v "$(pwd):/home/project:cached" theiaide/theia:next

Go to http://localhost:3000

Activate Command palette, (View -> Find command...) and use _Plugin: Deploy plugin by Id_

Provide _vscode:extension/camel-tooling.vscode-apache-camel_
