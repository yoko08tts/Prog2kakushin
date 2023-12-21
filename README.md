# Prog2kakushin
プログラミングⅡ課題⽤のリポジトリ

①pandasを用いたプログラム

◯プログラムの概要

・ToDoリストアプリです。いつまでに何をしなければいけないかをcsvファイルにメモすることができます。

・日付が近い順に自動的に並べてくれます。

・完了すればリストから削除することもできます。自分から削除しなくても、期限を過ぎると自動的にリストから削除してくれます。

・ToDoリストはGoogle Driveに保存されます。

◯どんな状況で使うのか

・課題の提出期限などのメモ、確認に使えると思います。

◯入力と出力

・「path」でGoogle Driveのどこに保存するか、またはどこのファイルを開くか指定します。

・「file_name」で保存する、または開くcsvファイルの名前を指定します。

・「purpose」でモードを選択できます。

「表示」モードではToDoリストを見ることができます。

「追加」モードでは「date」で期限を、「to_do」で何をするのかを指定することで、それらをToDoリストに追加することができます。

「完了」モードでは「date」で期限を、「to_do」で何が完了したのかを指定することで、それらをToDoリストから削除することができます。

◯工夫した点

期限を過ぎると自動的にリストから削除する機能を実装するために、datetimeモジュールを使用しました。
