# css関連メモ

###  縁取り文字の表現の仕方

・text-stroke  
テキストに縁(ストローク)をつけてくれるプロパティ。テキストの境界線を中心に、内外両方に縁がつく。小さい文字や太い縁をつけると文字が潰れる可能性あり。

・text-shadow  
テキストに影をつけるプロパティ。テキストの外側に影がつく。縁の幅が大きくなると、テキストの角部分が不自然になる。


参考資料
https://wk-partners.co.jp/homepage/blog/hpseisaku/htmlcss/huchidorimoji/


###  Flexboxの使い方

Flexboxは親要素(コンテナ)と子要素(アイテム)で構成される。  

(使い方)

①HTMLに親要素を作成しその中に子要素を作成する。
②cssで親要素にdisplay:flex;を指定。
③細かなレイアウトを指定する時は、親要素・子要素にそれぞれプロパティを指定する。  

「親要素に指定できるプロパティ」

flex-direction - アイテムの並び順を指定する
flex-wrap - アイテムの折り返しを指定する
flex-flow - アイテムの並び順と折り返しを一括で指定する
justify-content - アイテムの水平方向の位置を指定する
align-items - アイテムの垂直方向の位置を指定する
align-content - アイテムの行の垂直方向の位置を指定する

「子要素に指定できるプロパティ」

order - アイテムの並び順を指定
flex-grow - アイテムの伸び率を指定
flex-shrink - アイテムの縮み率を指定
flex-basis - アイテムのベースの幅を指定
flex - アイテムの伸び率、縮み率、ベースの幅を一括指定
align-self - アイテムの垂直方向の位置を指定


参考資料
https://webdesign-trends.net/entry/8148
