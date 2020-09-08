# Google Search Focus - Firefox Add-ons
👽 Remove "People also search for(PASF)" in Google Search on Firefox Add-ons.
Googleの「他の人はこちらも検索」を非表示にするFirefoxのアドオンです。

## Firefox Add-ons URL
[Google Search Focus - Firefox Add-ons](https://addons.mozilla.org/ja/firefox/addon/google-search-focusing/)

## Technologies
CSS Only.

## Thankyou
### Icons
[Dragon game glass series spear thrones weapon icon](https://www.iconfinder.com/icons/4527381/dragon_game_glass_series_spear_thrones_weapon_icon)

## CHNAGELOG
### v1.2.1
- Feat
  - Block "People also search for(PASF)" for Ad area. 広告エリアに表示される「他の人はこちらも検索」にも対応しました。ただし、きれいにブロックできておらず、一瞬だけ下に伸びて（約5px〜10px程度）また元に戻る挙動になります。これは「他の人はこちらも検索」が表示される際に、JavaScriptで下にベローンとスクロールするアニメーションが効いているのですが、そのアニメーションを無効化できていないためです。こちらについては対応方法を調査中です。

### v1.2.0
- Feat
  - Support to Smartphones browsing(only emulator). ブラウザのエミュレーターでスマートフォン表示した場合に対応しました。

### v1.1.0
- Fix
  - Fixed for changing Google source. Google側のソースが変更されたため、それに対応しました。

### v1.0.1
- Fix
  - Show icons in Add-ons Manager
  - Delete unused source code (main.js)

### v1.0.0
First release.
