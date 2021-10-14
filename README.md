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
### v1.2.2
枠が非表示にできない課題に暫定対応しました。  

■新たな課題の現象  
完璧な対応にはなっておらず、一瞬だけ枠が表示されます。  

■課題の原因  
Googleの仕様として「Webサイトの描画後に、JavaScriptを使って枠をゆっくり展開表示する」という挙動を実装しています。本アドオンでは「CSSでGoogleが枠を表示しなかったものにする」という命令を付け加えることで、枠を非表示にしています。  
JavaScriptとCSSでは、JavaScriptの命令のほうが強いため、CSSの命令が遅れて反映されてしまうため、一瞬だけ枠が表示されてしまいます。  

■（参考）用語説明  
JavaScript：Webサイトの挙動が変更できる仕組み  
CSS：Webサイトの見た目（デザイン）が変更できる仕組み  

■備考  
本アドオンは、CSSのみを使っているのですが、CSSで対応できる範疇の限界のようでした。  
本来はJavaScriptを利用すれば、ほかに対応策も考えられるのですが、JavaScriptは挙動自体が変更できてしまうため、良いことも悪いこともできます。キュリティ上の観点より、可能な限りJavaScriptは利用すべきではないと考えているため、やむをえずCSSのみを利用した片手落ちの実装となりました。  

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
