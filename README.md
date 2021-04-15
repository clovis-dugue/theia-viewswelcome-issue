# HOWTO Reproduce

1. Open this project in VS Code
2. Run the extension in the development host (e.g. by using F5)
3. Bring up the contributed view and observe the presence of the `viewsWelcome` content
5. Close the development host
6. Package the extension to a VSIX file using `vsce package`
7. Install this VSIX onto Theia and repeat 3 ; the `viewsWelcome` content is not here

## Noteworthy environment details

The extension is developped in TypeScript, and packaged using Webpack ; all from VSCode's generator using `yo code` and specifying this environement. The same issue occurs even when not using Webpack
