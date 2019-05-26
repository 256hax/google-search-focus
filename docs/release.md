# Release
## 1. Test
[Your first WebExtension > Testing](https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Your_first_WebExtension#Testing)

## 2. Packaging and Lint
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

## 3. Publish to Firefox Add-ons
Go to [ddons.mozilla.org (AMO)](https://addons.mozilla.org/ja/developers/addon/submit/distribution)

## 4. Release to GitHub
1. Go to [GitHub Releases](https://github.com/256hax/google-search-focus/releases)
2. Creat a new release. Then upload release zip file.
