---
title: "モデルについて"
description: ""
custom_edit_url: null 
sidebar_position: 3
---

# モデルについて

## 説明

モデルは、主に絵柄に影響する

- デフォルトではBNOM（BloodNightOrageMix）が指定される

- まずはALLで絵柄を確認するのがおすすめ

## モデル一覧

|モデル名|イラスト傾向|ソース|バージョン等|
|:--|:--|:--|:--|
|A1_Counterfeit|陰影が強い　顔や背景が特に精細|[Hugging Face](https://huggingface.co/gsdf/Counterfeit-V2.5)|V2.5|
|A2_BreakDomainAnime|リアル寄りアニメ風　メカや建物に強い|[Civitai](https://civitai.com/models/72675/breakdroidanime)|_a0440|
|A3_ShiratakiMix|動きがある構図が出やすい
|[Hugging Face](https://huggingface.co/Vsukiyaki/ShiratakiMix)|fixed|
|||||
|B1_BNOM（デフォルト）|強い特徴がなく、高い完成度|||
|B2_Kawaiiniji|繊細な線　珍しい構図が出やすい|[Civitai](https://civitai.com/models/52922/kawaiiniji)|v3|
|B3_El_Dorado|比較的平面的なイラスト|El Dorado.safetensors|[Hugging Face](https://huggingface.co/deadman44/SD_Anime_Merged_Models)|無印|
|||||
|C1_CuteYukiMix|SDとイラストの中間点|[Civitai](https://civitai.com/models/28169/cuteyukimix)|v3.0|
|C2_KawAICE|かなりSD寄り　淡い色使い|[Civitai](https://civitai.com/models/51057/aice-or-kawaice)|Channel|
|C3_threeAB|はっきりSD　塗りや線が強い|[Hugging Face](https://huggingface.co/sleepotimer/Model_A)|3AB|
|||||
|ALL|モデルだけ変えて9枚生成|||

## その他

- Aは繊細、Bは平均的、CはSDっぽい傾向にしているので、その間でいろいろ試すといい
  
- ALLのときの画像は以下の順<br/>
  A1 A2 A3<br/>
  B1 B2 B3<br/>
  C1 C2 C3

- ALLについては、同じシードで似にくいモデルを選んでいるので、比較にならないこともあるかも

- 他のモデルで試したいのがあれば教えてください
