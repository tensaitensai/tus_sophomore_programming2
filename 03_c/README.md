課題 以下のプログラムをそれぞれ組むこと．\
課題１ 二重線形リストを用いた選択ソートの実装
ファイルからデータ（数値の個数 N および N 個の整数値）を読み込み，以下の方針で昇
順にソートする（リストを利用した選択ソート）．\
リストは二重線形リストとし，その実装は配列を用いる．
1. 数値の個数 N を読みんだ後， この整数を読み込み，配列 Data に格納する．
2. 以下の操作を i=0 から N−1 までくり返す
Data[i] に格納された整数を key としてもつセルを作成してリストの先頭に挿入する．
3. 以下の操作を i=0 から N−1 までくり返す
リストの中の key の値が最小であるセルをを見つけ，その key の値を Data[i] に格
納してセルをリストから削除する
4. 配列 Data に格納された値を順に出力する
   
課題２ 線形リストを用いた選択ソートの実装\
課題１と同じ手続きを，線形リスト（prev を保持しないリスト）を用いて実装する．\
リストを配列で実装するプログラムを組む際の注意
- リストは構造体 struct を定義した上で配列で実現すること．
- リストや head の値を関数の引数にするときはポインタ渡しにすること．
- 空きアドレスを管理するようにすること．すなわち，挿入する際には allocate object で
空きアドレスを取得し，削除したセルは free object で空きアドレスのリストに戻すこと．