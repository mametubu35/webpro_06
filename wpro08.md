##私の好きな〇〇一覧

<!--
好きな曲　アーティスト名　再生回数　URL
好きな実況者一覧 チーム名　youtube登録者数　動画本数 URL
好きなVtuber一覧　会社名　youtube登録者数　動画本数 URL

好きな曲
d1　プロポーズ
d2　ダーリン
d3　ラヴィ
d4　モエチャッカファイア
d5　一旦ステイ Tonight
d6　パイナップルパーク
d7　シャルル

好きな実況者
d1　らっだぁ
d2　ぺいんと
d3　ぐちつぼ
d4　ととみっくす
d5　nquse
d6　
d7
-->





```mermaid
stateDiagram-v2
    [*] --> /public/sukina.html
    /public/sukina.html --> /jikkyou
    /public/sukina.html --> /Vtuber
    /public/sukina.html --> /kyoku
    /public/sukina.html --> /jouhou
    /jikkyou --> /view/jikkyou.ejsによる一覧表示
    /Vtuber --> /view/vtuber.ejsによる一覧表示
    /kyoku --> /view/kyoku.ejsによる一覧表示
    /jouhou --> /view/jouhou.ejsによるデータ関連一覧表示
    /view/jouhou.ejsによるデータ関連一覧表示 -->/sakujo
    /view/jouhou.ejsによるデータ関連一覧表示　-->/henkou
    /view/jouhou.ejsによるデータ関連一覧表示 --> /touroku
    /sakujo --> /view/sakujo.ejsによるデータ削除
    /henkou --> /view/henkou.ejsによるデータ変更
    /touroku --> /view/touroku.ejsによるデータ登録
    /view/touroku.ejsによるデータ登録 --> /view/vtuber.ejsによる一覧表示
    /view/touroku.ejsによるデータ登録 --> /view/jikkyou.ejsによる一覧表示  
    /view/touroku.ejsによるデータ登録 --> /view/kyoku.ejsによる一覧表示 
    /view/henkou.ejsによるデータ登録 --> /view/vtuber.ejsによる一覧表示
    /view/henkou.ejsによるデータ登録 --> /view/jikkyou.ejsによる一覧表示  
    /view/henkou.ejsによるデータ登録 --> /view/kyoku.ejsによる一覧表示 
    /view/sakujo.ejsによるデータ登録 --> /view/vtuber.ejsによる一覧表示
    /view/sakujo.ejsによるデータ登録 --> /view/jikkyou.ejsによる一覧表示  
    /view/sakujo.ejsによるデータ登録 --> /view/kyoku.ejsによる一覧表示 
    

```