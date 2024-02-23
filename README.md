# @osaxyz/universtyle

## インストール

`npm install @osaxyz/universtyle`

## どう動くか

`harmonic()`で調和数列に基づくサイズを取得、`fibo()`でフィボナッチ数列に基づくサイズを取得、`silver()`で白銀比に基づくサイズを算出できます。

## 使い方

### scoped styleの場合

```sass
@use "@osaxyz/universtyle" as osa

html
    font-size: 16px

body
    font-size: osa.harmonic(1)

h1
    font-size: osa.harmonic(3)
    line-height: osa.silver(osa.harmonic(3), 1)
```