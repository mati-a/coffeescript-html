# CoffeeScript HTML (coffeescript-html)

## Features

VSCode extension to highlight HTML in CoffeeScript files.

## Extension Settings

To install go to `Extensions` -> `(Three dots)` -> `Install from VSIX...` and select the file on `releases` folder.

### AngularJS

You can highlight AngularJS (like custom elements or angularjs specifics) using this on you `.vscode/settings.yml`:

``` json
{
    "editor.tokenColorCustomizations": {
        "textMateRules": [
            {
                "scope": "meta.attribute.unrecognized entity.other.attribute-name.html",
                "settings": {
                    "foreground":"#DCDCAA"
                }
            },

            {
                "scope": "meta.tag.custom entity.name.tag.html",
                "settings": {
                    "foreground": "#4EC9B0"
                }
            },
            {
                "scope": [
                    "meta.attribute.unrecognized.ng-switch entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-switch-when entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-if entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-class entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-submit entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-model entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-show entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-disabled entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-click entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-repeat entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-model-options entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-attr-maxlength entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-switch-default entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-pattern entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-style entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-hide entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-transclude entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-repeat-start entity.other.attribute-name.html",
                    "meta.attribute.unrecognized.ng-repeat-end entity.other.attribute-name.html"
                ],
                "settings": {
                    "foreground":"#C586C0"
                }
            }
        ]
    }
}
```

To see the elements and current color you can use the command `Developer: Inspect Editor Tokens and Scopes` (Cmd + Shift + P)

## Generate release file

`vsce package`

## Release Notes

### 0.0.1

Initial release
