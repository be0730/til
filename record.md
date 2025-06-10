rakeタスク
久々に応用カリキュラムに戻り、再開しようとしたところ...
・bin/devが起動しない
　GPTに聞いてみるとスペルミス＆構文のエラーとのこと
 そのため下記のように修正
 （中途半端なところで止めていたから書いた記憶も全くなく焦る💦）
'''
【Rails.root/lib/tasks配下に拡張子.rakeで保存する】
　namespace :hoge do
  desk 'タスクの説明' 　　→　 desc 'タスクの説明'
  task task_name: do　　→　 task task_name: :environment do　#task_nameは自由に設定できる
    #実行したい処理　　　　　　　#実行したい処理
  end                      end
end                       end
'''


