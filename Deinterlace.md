# Deinterlace from [ffmpeg-filters](https://ffmpeg.org/ffmpeg-filters.html)

## 11.16 bwdif

入力した動画をインタレ解除します。("bwdif"は"Bob Weaver Deinterlacing Filter"の略)

w3fdifとcubic interpolationアルゴリズムを利用したyadifをベースとした**動きに最適な**インタレ解除。

## 11.110 kerndeint

入力した動画をDonald Graftの最適なカーネルインタレ解除を適用することでインタレ解除します。動画のインターレースされた部分で動き、progressiveなフレームを提供する。

## 11.138 nnedi

動画をneural network edge directed interpolationを使ってインタレ解除します。

## 11.233 w3fdif

入力した動画をインタレ解除します。("w3fdif"は"Weston 3 Field Deinterlacing Filter"の略)

BBC R&DのためにMartin Westonが説明したプロセスをベースにして、BBC R&DのためにJim Easterbrookが書いたインタレ解除アルゴリズムをベースに実装して、Westonの3 fieldインタレ解除フィルターはBBC R&Dによって計算されたフィルターcoefficientsを利用する。

このフィルターはフレーム内にあるfield-dominance情報をそれぞれのペアのどちらを先に出力するかを決めるのに使う。もしそれが失敗したら、w3fdifフィルターの前にsetfieldフィルターを利用する。

## 11.240 yadif

入力した動画をインタレ解除します。("yadif"は"yet another deinterlacing filter"を意味)
