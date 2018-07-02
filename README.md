# processing

実行した処理はエッジの検出です。
pythonのOpenCVを使っています。

参考にしたサイトは「http://www.non-fiction.jp/2015/08/15/edge-detect-laplacian/　」
また画像の表示を行う部分は前回と同じものを使用しました。

9～11行目を引用しています。

9行目はopenCVのGaussianフィルタを利用して平滑化
10行目でLaplacianフィルタをかけて 
11行目で8ビット符号なし整数に変換しています。
