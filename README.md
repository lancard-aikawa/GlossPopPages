# GlossPop Pages

[GlossPop](https://github.com/lancard-aikawa/GlossPop) で書き出した用語辞書の公開ページ。
GitHub Pages で公開している → **https://lancard-aikawa.github.io/GlossPopPages/**

ここが持つのは **書き出した成果物だけ**。辞書の中身（`.glosspop/`）と本文は
それぞれのプロジェクトに置いたままで、ページからは何も参照していない
（本文も辞書も 1 枚ずつに焼き込んであるので、**サーバが無くても読める**）。

## 1 つ足す

GlossPop のビューアで、そのフォルダを開いてから:

1. ⚙ → **公開** で、書き出し先をこのリポジトリのフォルダに、
   URL を `https://lancard-aikawa.github.io/GlossPopPages/` にする
2. 上のバーの **⋯ → 🌐 公開する…** → カードを確かめて **書き出す**
3. `index.html`（このファイルの隣）に 1 行足す
4. `git add -A && git commit && git push`

**カードの画像は URL に `?v=<中身の印>` が付く。** X はカードを URL ごとに
覚えていて確実に更新させる手段が無いので、中身が変わったときだけ URL が変わる
仕掛けになっている（同じ内容で撮り直しても無駄にキャッシュを切らない）。

## いま置いてあるもの

| | |
| --- | --- |
| [戦国時代](https://lancard-aikawa.github.io/GlossPopPages/%E6%88%A6%E5%9B%BD%E6%99%82%E4%BB%A3/) | 史実と諸説の並記を試した辞書（25 語 / 関係 40 本）。素材は [GlossPop の samples](https://github.com/lancard-aikawa/GlossPop/tree/main/samples/%E6%88%A6%E5%9B%BD%E6%99%82%E4%BB%A3) |

## GitHub Pages の設定

Settings → Pages → Source = **Deploy from a branch**、Branch = `main` / `(root)`。
ビルドは無く、置いたファイルがそのまま配信される（`.nojekyll` があるので
Jekyll は通らない）。
