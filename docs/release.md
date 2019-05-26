# Release
## Test
[Your first WebExtension > Testing](https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Your_first_WebExtension#Testing)

## Packaging and Lint
### Packaging
```
$ cd [PJ root directory]
```

manifest.json should be put in root.

```
$ cd dist
$ zip -r ../dist.zip ./* -x *.DS_Store
```

### Lint
```
$ cd [PJ root directory]
$ addons-linter dist.zip
```

## Publish to Firefox Add-ons
### Submission
Go to [ddons.mozilla.org (AMO)](https://addons.mozilla.org/ja/developers/addon/submit/distribution)
