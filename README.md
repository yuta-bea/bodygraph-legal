# 利用規約・プライバシーポリシー（GitHub Pages で公開する）

**Appleの審査ではプライバシーポリシーのURLが必須。** 利用規約もペイウォールからリンクする。

## 公開手順

1. GitHub で新しいリポジトリを作る（例: `bodygraph-legal`）。**Public にする**
2. このフォルダの4ファイルを push する
   - `index.html` / `terms.html` / `privacy.html` / `style.css`
3. リポジトリの **Settings → Pages**
   - Source: `Deploy from a branch`
   - Branch: `main` / `/ (root)` → Save
4. 数分待つと以下のURLで公開される

```
https://yuta-bea.github.io/bodygraph-legal/terms.html      利用規約
https://yuta-bea.github.io/bodygraph-legal/privacy.html    プライバシーポリシー
https://yuta-bea.github.io/bodygraph-legal/support.html    サポート（App Store Connect の必須項目）
```

## 公開後にやること

**この2つのURLをCEOに渡す。** `app/src/lib/config.ts` の `TERMS_URL` と `PRIVACY_URL` に入れる。
**JSの値なのでリビルドは不要。**

## 連絡先

`yutabation@gmail.com`（2026-08-20 に4ファイルへ記載済み）

**Appleの審査で連絡先が確認される。** 変更する場合は
`index.html` / `terms.html` / `privacy.html` / `support.html` の4ファイルすべてを直すこと。

## 中身について

- **医療上の助言ではない**旨を規約2章に明記した。筋力の目標を表示するアプリなので、ここは外せない
- **ランクは目安であり、基準を見直すことがある**旨を3章に明記した。実際、レベル基準表は今後変える可能性が高い
- サブスクリプションの自動更新・解約方法（4章）は**Appleが表示を要求している項目**
- OpenPowerlifting と react-native-body-highlighter（MIT）の帰属表示を9章に入れた
