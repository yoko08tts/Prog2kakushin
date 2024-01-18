# Prog2kakushin

# ①pandasを用いたプログラム
- プログラムの概要
  - ToDoリストアプリです。いつまでに何をしなければいけないかをcsvファイルにメモすることができます。
  - 日付が近い順に自動的に並べてくれます。
  - 完了すればリストから削除することもできます。自分から削除しなくても、期限を過ぎると自動的にリストから削除してくれます。
  - ToDoリストはGoogle Driveに保存されます。

- どんな状況で使うのか
  - 課題の提出期限などのメモ、確認に使えると思います。

- 入力と出力
  - 「path」でGoogle Driveのどこに保存するか、またはどこのファイルを開くか指定します。
  - 「file_name」で保存する、または開くcsvファイルの名前を指定します。
  - 「purpose」でモードを選択できます。
  - 「表示」モードではToDoリストを見ることができます。
  - 「追加」モードでは「date」で期限を、「to_do」で何をするのかを指定することで、それらをToDoリストに追加することができます。
  - 「完了」モードでは「date」で期限を、「to_do」で何が完了したのかを指定することで、それらをToDoリストから削除することができます。

- 工夫した点
  - 期限を過ぎると自動的にリストから削除する機能を実装するために、datetimeモジュールを使用しました。

# ②numpyを用いたプログラム
- プログラムの概要
  - 相対音感クイズをすることができるアプリです。
  - プログラムを実行すると、２つの音がなります。最初に鳴った音を「ド」とすると、次の音はなんの音になるか、というクイズです。

- どんな状況で使うのか
  - 自分の音感を試したり鍛えたりするために使えると思います。

- 入力と出力
  - key_tonic で最初になる音(主音)を設定できます。
  - key_scale で問題に出る音階を設定できます。
  - 例えば key_tonic を「D」、key_scale を「major」に設定してプログラムを実行すると、最初に「D」の音が鳴り、次に「D」「E」「F#」「G」「A」「B」「C#」のいずれかの音が鳴ります。
  - answer で答えを選択してからプログラムを実行すると、答え合わせをすることができます。

- 工夫した点
  - n半音上がるたびに周波数が 2^(n/12) 倍になることと、numpyの累積和を求める機能を利用して、色々な音階を作れるようにしました。

# ③画像処理を用いたプログラム
- プログラムの概要
  - モザイクアートメーカーです。
  - モザイクアートにしたい画像とモザイクアートを作る素材となる画像が入ったフォルダをcolab内にアップロードすると
    
    モザイクアートを作ることができます。

- どんな状況で使うのか
  - モザイクアートを作って遊べると思います。

- 入力と出力
  - 変数 d を変更するとモザイクアートに使われている画像一つひとつの大きさを変更できます。
  - 例えば d を 4 に設定すると画像一つひとつの大きさが 4ビット × 4ビット になります。
  - file_path でどの画像をモザイクアートにするか指定できます。モザイクアートにしたい画像のパスを入力してください。
  - folder_pathでモザイクアートを作る素材となる画像を指定できます。その画像がすべて入ったフォルダを用意し、そのパスを入力してください。
  - これらを正しく入力するとモザイクアートが生成されます。


- 工夫した点
  - モザイクアートを作るために、画像をいくつもの領域に分けて処理をするプログラムを作成しました。
