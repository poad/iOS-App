# iOS-App

1. Apple Developer Program 登録する
2. キーチェーンアクセス アプリから、証明書要求を作成する
3. Xcode から `Apple Developer` の証明書を作成する
4. Apple Developer Program Membersip から、上述の証明書を使った Provisioning Profile を作成する
5. Xcode で Provisioning Profile をダウンロードする
6. `ls ~/Library/MobileDevice/Provisioning\ Profiles/` で、 Provisioning Profile の UUID を確認する
7. exportOptions.plist に Provisioning Profile の UUID を記述する
8. Xcode から証明書を export する
9. `cat "p12 ファイル名" | base64` の結果を取る
10. GitHub Secrets に上述の BASE64 エンコード済の p12 ファイルの内容を登録する
