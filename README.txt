旅プランナー Android APK化用 PWA ソース

1. GitHubで新規リポジトリ travel-planner を作成します。
2. このフォルダの中の index.html、manifest.webmanifest、sw.js、icon-192.png、icon-512.png をリポジトリ直下にアップロードします。
3. GitHub Settings > Pages > Deploy from a branch > main / (root) > Save。
4. https://<GitHubユーザー名>.github.io/travel-planner/ が開くことを確認。
5. Windows PowerShellで npm install -g @bubblewrap/cli を実行。
6. bubblewrap init --manifest https://<GitHubユーザー名>.github.io/travel-planner/manifest.webmanifest
7. 案内に従ってAndroid SDK/JDK、署名鍵などを設定し、bubblewrap build を実行。
8. 生成したAPKをAndroidへ転送してインストール。

注意: 本ZIPにAPKは含まれません。Googleカレンダー自動同期は未実装です。
保存データは端末のブラウザストレージに依存します。消去・機種変更で失われる可能性があります。
