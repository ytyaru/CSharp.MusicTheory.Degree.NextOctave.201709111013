# このソフトウェアについて

C#で音度からピッチクラスを取得する（複音程に対応した）。

複音程に対応したため、正確にはピッチクラスではなく「第一音からの半音数」を取得する。取得値を`v`としたとき、`(v % 12)`とすればピッチクラスを取得できる。

# 前回

* https://github.com/ytyaru/CSharp.MusicTheory.Chord.201709101113
* https://github.com/ytyaru/CSharp.MusicTheory.Chord.Accidential.201709101700

# Python版

* [和音名(ChordName)から構成音を音程名(IntervalName)で取得する](http://ytyaru.hatenablog.com/entry/2018/10/04/000000)

Python版で書いていたが、音楽理論の難しさとPython言語での実装に限界を感じた。現在C#に移植中。

# 課題

* `+-#b♯♭1`のように異なる変化記号も併用できてしまう
    * `++1`など同一の記号を連続する使い方のみに限定したいが、スマートな実装方法が見つけられなかったので放置する

# 開発環境

* Linux Mint 17.3 MATE 32bit
* [MonoDevelop 4.0.12](http://ytyaru.hatenablog.com/entry/2018/05/25/000000)
* [mono 3.2.8](http://ytyaru.hatenablog.com/entry/2018/05/24/000000) (Debian 3.2.8+dfsg-4ubuntu1.1)
    * mcs(Mono C# compiler) 3.2.8.0
    * csharp(インタプリタ) 4.0.0.0

# ライセンス

このソフトウェアはCC0ライセンスである。

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.ja)

