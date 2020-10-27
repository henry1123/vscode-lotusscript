# VSCode LotusScript

[![Marketplace Version](https://vsmarketplacebadge.apphb.com/version/henry1123.lotusscript.svg)](https://marketplace.visualstudio.com/items?itemName=henry1123.lotusscript)
[![Installs](https://vsmarketplacebadge.apphb.com/installs/henry1123.lotusscript.svg)](https://marketplace.visualstudio.com/items?itemName=henry1123.lotusscript)
[![Rating](https://vsmarketplacebadge.apphb.com/rating/henry1123.lotusscript.svg)](https://marketplace.visualstudio.com/items?itemName=henry1123.lotusscript)

<!-- TOC depthFrom:2 -->

- [VSCode LotusScript](#vscode-lotusscript)
  - [Syntax Highlighting](#syntax-highlighting)
  - [Snippets](#snippets)
    - [Basic code](#basic-code)
  - [Installation](#installation)
  - [Contributing](#contributing)
  - [Contacts](#contacts)
  - [Links](#links)
  - [Handy links](#handy-links)
  - [Version history](#version-history)

<!-- /TOC -->

## Syntax Highlighting

This package provides syntax highlighting and snippets of LotusScript.

Based off an import of the
[VSCode VBA](https://github.com/spences10/vscode-vba)
file from the
[Spences10.VBA](https://github.com/spences10/vscode-vba)
repository.

## Snippets

### Basic code

- dim declarations
- if/else
- for/while
- sub/function with errHandler
- case

## Installation

Launch VS Code Quick Open (Ctrl+P), paste the following command, and
press enter.

```
ext install lotusscript
```

## Contributing

Please fork this repository and contribute back using pull requests.

Any contributions, large or small, major features, bugfixes and
integration tests are welcomed and appreciated but will be thoroughly
reviewed and discussed.

## Contacts

You can contact me in the following ways:

- Mail : [henry1123@gmail.com](mailto:henry1123@gmail.com)
- Github : [henry1123](https://github.com/henry1123)

## Links

- [Source Code](https://github.com/spences10/vscode-vba)
- [Market](https://marketplace.visualstudio.com/items?itemName=spences10.VBA)

## Handy links

I struggled to find how to generate a token after not doing anything
with this project for well over a year:

To get to your token creation, go here:

- https://YOUR_USER_NAME.visualstudio.com/_details/security/tokens

**Create a token:**

- Name: vsce
- Organisation: All accessible organizations
- show all scopes, select:
  - Marketplace
    - Check Acquire and Manage

**Publish with CLI:**

```bash
# login
vsce login <publisher name>
vsce package
# myExtension.vsix generated
# bump version
vsce publish minor # | major | patch
# vsce publish major, minor or patch
vsce publish -p <add created token here>
```

If you get `ERROR Failed request: (401)` see here:

- https://github.com/Microsoft/vscode-vsce/issues/11

Some good documentation on publishing with the CLI:

- https://code.visualstudio.com/api/working-with-extensions/publishing-extension

## Version history

```
20200405 - Added basic If snippet, and changed all snippets to use tabs (for user customisation capability).
20200405 - Multi-line comment capability
20200405 - Added certain keywords e.g. Type, Enum, Implements, Optional, Friend, ... Also changed behavior of some keywords, e.g. "End","Function","Sub" instead of "End Function", "End Sub" etc..
20200405 - Removal of non-vba behavior.
20200714 - [Comment with REM].
```

<!-- Links -->
[Comment with REM]:https://github.com/spences10/vscode-vba/pull/13