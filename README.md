【システム要件】

　＜ログイン認証＞
　　画面１：ログイン画面
　　　IDとPassでログインをする
　　　DBと照合し、登録済みの場合は画面２へ遷移し、
　　　その他の場合は適したエラー文言を同画面に表示する。
　　画面２：ログイン後のTOP画面
　　　ログインIDの表示をする
　　テスト：JUnitを利用し、DAOのテスト
　　　　　　入力項目のテスト

　＜ユーザ情報更新＞
　　画面３：ユーザ情報更新画面
　　　画面２から遷移し、ユーザ情報を表示、更新可能にする。
　　　表示項目：ID・Pass・ユーザ名・メールアドレス・電話番号
　　　入力時はバリデーションを用いる
　　　IDのみ更新不可
　　　ID＋Passテーブルとは別のユーザテーブルを作成する
　　画面４：更新内容確認画面
　　　画面３から遷移し、更新内容を表示する。
　　　更新完了後は、画面２に遷移。
　　上記同様テストの実施

　＜ユーザ登録＞
　　画面５：ユーザ登録画面
　　　画面２から遷移し、新規ユーザを登録可能にする。
　　　IDは自動採番、その他は入力。
　　画面６：登録内容確認画面
　　　画面５から遷移し、登録内容を表示する。
　　　更新完了後は、画面２に遷移。
　　上記同様テストの実施

　＜ユーザ削除＞
　　画面７：ユーザ削除画面
　　　画面２から遷移し、ユーザ一覧を表示し削除を可能にする。
　　　ログインユーザは表示されるが、削除不可。
　　　複数ユーザ同時削除可能にする。
　　画面８：ユーザ削除確認画面
　　　画面７から遷移し、削除ユーザIDとユーザ名を表示する。
　　　削除完了後は、画面２に遷移。
　　上記同様テストの実施

私はイヌ派
私はneko派 ←new!!

