# Release
## 1. Test
Go to `about:debugging` in Firefox browser. Move to "This Firefox" > "Load Temporary Add-ons" then, drag&drop your some files in Firefox Add-ons directory(ex: "manifest.json").

More details - [Your first WebExtension > Testing](https://developer.mozilla.org/ja/docs/Mozilla/Add-ons/WebExtensions/Your_first_WebExtension#Testing)

## 2. Packaging and Lint
### Packaging
```
$ cd [PJ root directory]
```

manifest.json should be put in root.

```
$ cd dist
$ rm ../dist.zip
$ zip -r ../dist.zip ./* -x *.DS_Store
$ zipinfo ../dist.zip
```

### Lint
```
$ cd [PJ root directory]
$ addons-linter dist.zip
```

## 3. Publish to Firefox Add-ons
Go to [ddons.mozilla.org (AMO)](https://addons.mozilla.org/ja/developers/addon/submit/distribution) then, Upload New Version.

## 4. Release to GitHub
1. Go to [GitHub Releases](https://github.com/256hax/google-search-focus/releases)
2. Creat a new release. Then upload release zip file.
