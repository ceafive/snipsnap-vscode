# Snipsnap - ultimate snippet handler for Visual Studio Code

[Snipsnap](https://snipsnap.dev/) is unopionated ultimate snippet handler that automatically exposes to you all available snippets for every library you are using in your project. Spend your time building great things, not orchestrating snippet extensions.

<p align="center">
  <em>
    JavaScript
    · Python
    · PHP 
    · Go 
    · Java 
  </em>
  <br />
  <em>
    Node
    · Flask 
    · Spring 
  </em>
  <br />
  <em>
    HTML
    · Vue
    · React
    · Rails
  </em>
  <br />
  <em>
   <strong>Literally any library in any programming language</strong> 
  </em>
  <br />
  <em>
    <a href="https://snipsnap.dev/add">
      Would like to see a particular library?
    </a>
  </em>
</p>

<p align="center">
  <a href="https://drone.pixelpoint.io/snipsnapdev/snipsnap-vscode"><img src="https://img.shields.io/drone/build/snipsnapdev/snipsnap-vscode/drone?server=https%3A%2F%2Fdrone.pixelpoint.io" /></a>
  <a href="https://marketplace.visualstudio.com/items?itemName=snipsnapdev.snipsnap-vscode">
    <img alt="VS Code Marketplace" src="https://img.shields.io/visual-studio-marketplace/v/snipsnapdev.snipsnap-vscode"></a>
  <a href="https://marketplace.visualstudio.com/items?itemName=snipsnapdev.snipsnap-vscode">
    <img alt="VS Code Marketplace Downloads" src="https://img.shields.io/visual-studio-marketplace/d/snipsnapdev.snipsnap-vscode"></a>
  <a href="https://marketplace.visualstudio.com/items?itemName=snipsnapdev.snipsnap-vscode">
    <img alt="VS Code Marketplace Installs" src="https://img.shields.io/visual-studio-marketplace/i/snipsnap-vscode"></a>
   
</p>

## Installation

Install through VS Code extensions. Search for `Snipsnap - Snippets Handler`

[Visual Studio Code Market Place: Snipsnap - snippets handler](https://marketplace.visualstudio.com/items?itemName=snipsnapdev.snippsnap-vscode)

Can also be installed in VS Code: Launch VS Code Quick Open (Ctrl+P), paste the following command, and press enter.

```
ext install snipsnap-vscode
```

## Configuration

No config required and more than that - no config even exists! You are good to go right after installing the extension.

## Usage

No manual activation required as well, the extension triggers if your workspace folder contains `package.json` file and does magic on its own, but if you still need to trigger it, use `Reload Window` in Command Palette.

## Settings

The only available configuration option is possibility to exclude certain libraries from snippets request.

Snipsnap works by gathering all deps throughout the project, even from lock files, so some of subdependencies like lodash could pollute your snippet environment and become a major frustrating factor.

To ensure that no `%unwanted_library%` snippets are being fetched, you should create `.snippetsignore.json` file at the root of your project and specify all libraries you want to be ignored in a single list, e.g.

```json
["react", "lodash", "html"]
```

## Error Messages

Reload using Command Paletter or just reload the window. If the problem hasn't dissapeared, please, [submit an issue with a description](https://github.com/snipsnapdev/snipsnap-vscode/issues).

## Telemetry

This extension respects the VS Code telemetry setting so if you have telemetry disabled in VS Code we will also not collect telemetry. See the [Visual Studio Code docs](https://code.visualstudio.com/docs/getstarted/telemetry#_disable-telemetry-reporting) for information on how to disable telemetry.

However, at this point 0 telemetry data is being gathered if you did not tweaked vscode telemetry settings.

## License

MIT
