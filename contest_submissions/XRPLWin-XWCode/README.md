# XWCode - JSHooks Builder
Native IDE for Web3 Development ([try it now](https://xahau.xrplwin.com/code/jshooks))

![xw1](https://github.com/user-attachments/assets/d5398cc4-5bbc-4125-a214-146165fd2bf7)


## Overview
The XWCode Core and Components are made from zero by XRPLWin in event-driven architecture. IDE components are extendable by plugins. "JSHooks Builder"
edition of this IDE is combination of specific plugins which gives Hooks build and deploy capabilities to the underlying core XWCode engine.

## Plugins
1. **Filesystem** - gives filesystem capabilities using IndexedDB
2. **Console** - displays console and translates VM output to browser
3. **Settings** - manager for encrypted ENV variables and other IDE settings
4. **XRPLConnector** - gives capability to connect to different XRPL compatible networks (Xahau, Xahau-Testinet, ...)
5. **JSHooks** - gives tools, methods, and actions to build TS code to Hook (API Version 1) deployable binary code
6. **JSHooksEasy** - easy UI mode for building and deploying in one go
7. **HookDeploy** - gives ability to deploy Hook via integrated wallet system (Xaman, seed, ...)
8. **Welcome** - plugin that displays welcome landing page
9. **Webcontainer** - NodeJS Virtual Machine engine which runs in Web browser

## Architecture
### Filesystem
Files are stored in your web browser and persisted in IndexedDB storage. Option to download full project is available (as .zip archive).
File manager tree is available to view and browse all files available.

### Virtual machine
To build hook from TS project, project needs to be bundled with *esbuild*, to make this tool available NodeJS VM is used.  
Virtual Machine uses *Node v18* to build JS Hooks. Engine that is running this is [Webcontainers](https://webcontainers.io/) by [StackBlitz](https://stackblitz.com/)

### Plugins
Event driven architecture of the IDE allows easy extensions to be installed to ide (plugin manager is planned for future releases).

## Networks
IDE supports multi-networks connections, you can switch between XAHAU Mainnet, XAHAU Testnet and XAHAU JSHooks Testnet, also there is localhost connection for own local node build.
- XAHAU Mainnet
- XAHAU Testnet
- XAHAU JSHooks Testnet
- LOCAL

## Building

Powerful context-menu tools gives you control over your code, use context menu to build hook bundle or get binary source easily.

![image](https://github.com/user-attachments/assets/dee899bd-dec0-47a7-a525-2b169833c995)


## Deploying
Deploy UI gives you control over SetHook transaction, review and set available parameters before deploying on your account. 
- Deploy JSHooks
- Deploy CHooks

![image](https://github.com/user-attachments/assets/9b40f22f-2a43-4a27-bc3f-6594a33f41af)

## Additional tools
Account manager (bundled with the XRPLWin Explorer) enables you to manage installed hooks on your account.
Easily modify installed hook (change triggers, clear namespace, add or remove parameters, ...)

Also uninstall hook with few clicks.

- modify hooks
- clear namespace
- change namespace
- remove or add parameters
- remove or add grants
- deinstall hook

![image](https://github.com/user-attachments/assets/97acb6d7-5599-4dc2-89c5-2fa30d7e8ed2)


## Project status
Currently in *Beta* (public testing)

## What is missing
**Test interface** Built-in Wallet manager, faucet and easy-to-use forms to run transaction types.  
**Code snippets** Library of code snippets to make hook building easy task  
**Knowledgebase** Explorable documentation (connected to official docs)  


