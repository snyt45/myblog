---
slug: vim_comment_in_out
title: Vimでプラグインを使わずにコメントアウト・コメントアウト解除する方法
date: 2022-03-18
---

[[Twitter]]で[[Vim]]の便利な小技を紹介しているツイートで知りました！

普段は、`C-v`で矩形選択 →`S-i`して文字列を挿入してコメントアウトしているのですが、こういうやり方もあるのかということで紹介させていただきます。

https://twitter.com/vim_tricks/status/1504089969157103616

`:norm {commands}`というコマンドを打つと、ノーマルモードで`{commands}`を実行するときと同じ挙動になるみたいです。

これをビジュアルモードと組み合わせると、プラグインなしでコメントアウト・コメントアウト解除ができます。

https://www.loom.com/embed/d17e8ef178e641ee9469663a2ef1f586

- コマンド
  - 説明
- `:norm i#`
  - `i#`をノーマルモードで実行する
- `:norm x`
  - `x`をノーマルモードで実行する
