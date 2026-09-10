<div align="center">

# XXD Panel 117｜細線淡彩余白誌

一つの視覚の核から、写真の主題と余白を演出し直す。

<a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <strong>日本語</strong> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

## サンプル展示

本项目已发布 8 张实际样片，图片文件位于 `assets/examples/`。

| sample-05 | sample-06 |
| --- | --- |
| ![sample-05](assets/examples/sample-05.png) | ![sample-06](assets/examples/sample-06.png) |
| sample-07 | sample-08 |
| ![sample-07](assets/examples/sample-07.png) | ![sample-08](assets/examples/sample-08.png) |
| sample-09 | sample-10 |
| ![sample-09](assets/examples/sample-09.png) | ![sample-10](assets/examples/sample-10.png) |
| sample-11 | sample-12 |
| ![sample-11](assets/examples/sample-11.png) | ![sample-12](assets/examples/sample-12.png) |

## 向いている場面と解決する課題

写真が雑然としていたり構図が平凡でも、残す価値のある何かがあれば、**Panel 117** は一つの核心テーマ、一つの視覚的な核、一つの感情的な関係を抽出し、細線、淡い平塗り、紙の質感、軽いコラージュによる小さな画面へ演出し直します。比較領域に実写を残しながら、意図的な余白でデザインを独立させます。

### こんな場合に

- 原物の識別性を保ち、主体の位置、大きさ、方向、切り取りを再設計したい。
- 物ごとの描き写しや雑然とした背景ではなく、少要素で強い主題を作りたい。
- 写実的な細部や滑らかなベクターより、細線、柔らかなパステル、呼吸する紙面が好き。
- 上下、左右、デザインのみ、複数比率、4端末壁紙、フォルダ一括に対応したい。

### 解決すること

- 複雑な素材から重要な視覚の核を選び、二次情報を削ります。
- 余白が正負の形、距離、非対称の均衡を構成します。
- 比較は各50%の2領域のみとし、第三帯や入れ子のパネルを作りません。
- 出力ごとに現在の原画像から独立した一回の生成を行い、中間結果を再転写しません。

## 使い方のコツ

- **まず一枚の見やすい写真から始める：** 主体・動作・関係が分かる画像を選んでから、出力形式と比率を決めます。
- **パラメータを一文でつなぐ：** 「上下 / 左右 / デザインのみ + 16:9 / 3:4 / スマホ壁紙」のように指定し、PC・タブレット・スマートウォッチのサイズも追加できます。
- **残したい内容を明示する：** 人物、物、動作、関係、文字を指定し、レイアウトを細かく縛りすぎずスタイルに任せます。
- **文字の方法を選ぶ：** 画像から自動生成、`--text exact --copy` で逐字固定、または `--text none` で文字なしにできます。
- **写真領域とデザイン領域を伝える：** 上下・左右では写真を残す側と再設計する側を指定し、デザインのみ・壁紙では全画面を再設計すると伝えます。
- **一枚で試してから一括処理する：** モード、比率、文字、言語を一枚で確認し、同じ設定をフォルダに適用します。比較しやすいよう一度に一つだけ変更します。

## 原文プロンプト · 5言語

[简体中文](references/original-prompt/zh-CN.md) · [English](references/original-prompt/en.md) · [日本語](references/original-prompt/ja.md) · [한국어](references/original-prompt/ko.md) · [العربية](references/original-prompt/ar.md)

中国語ファイルは原文を逐字保存し、実行時の唯一の創作・美的権威です。他4言語は完全で忠実な閲覧用翻訳です。左右など既定以外のモードを明示的に選んだ場合、アダプターは位置と寸法だけを変換し、美的要件は変えません。

**特徴語：** 一つの核心テーマ · 一つの視覚の核 · 一つの感情的関係 · 細線手描き · 淡い平塗り · 紙の質感 · 軽いコラージュ · 小さな章印 · 2–4色 · 大きな余白 · 細い手書き文字

## クイック判定

| 気になること | Panel 117 の答え |
|---|---|
| 平凡な写真でも使えるか | 抽出後に主体の大きさ、位置、方向、切り取りを再設計します。 |
| 原物を認識できるか | 代表的な輪郭、流れ、姿勢、視覚の記憶点を保ちます。 |
| 余白は単なる未描画部分か | 描画面積より明らかに大きく、距離と正負の形を積極的に構成します。 |
| サイズを柔軟にしたい | 一般比率、正確なピクセル、4モード、フォルダ一括に対応します。 |

## 4つの出力モード

- `top-bottom`：全幅の上下2領域のみ。実写を上、デザインを下に置き、各50%。
- `left-right`：全高の左右2領域のみ。実写を左、デザインを右に置き、各50%。上下構成へ回転しません。
- `design-only`：全画面を Panel 117 のデザイン翻訳にし、写真は見えない参照にします。
- `wallpaper-pack`：スマートフォン、iPad、デスクトップ、時計を端末ごとに生成。`linked` または `independent` を選べます。

モードと比率は複数指定できます。`1:1`、`3:4`、`4:3`、`4:5`、`5:4`、`2:3`、`3:2`、`9:16`、`16:9`、`21:9`、`5:7`、`7:5`、正確なピクセルに対応します。文字はプロンプト生成、指定文の逐字使用、なしから選べます。フォルダ入力では各画像を分離して処理し、PNGを一つの新しいタスクフォルダへ置きます。

## はじめに

```bash
git clone https://github.com/nevertoday/xxd-panel-117.git
npx skills add https://github.com/nevertoday/xxd-panel-117 --skill xxd-panel-117
```

インストール後に Agent セッションを再起動し、`$xxd-panel-117` を呼び出します。ユーザー単位の Codex には `--global --agent codex --yes` を追加できます。

```text
/xxd-panel-117 photo.jpg --mode top-bottom --size 3:4 --text prompt --locale ja-JP
/xxd-panel-117 photo.jpg --mode left-right --size 16:9 --text prompt --locale en-US
/xxd-panel-117 photo.jpg --mode design-only --size 9:16 --text none
/xxd-panel-117 ./photos --mode design-only --size auto,3:4 --text prompt --locale ja-JP
```

完全な実行契約は [SKILL.md](SKILL.md)、実行アダプターは[英語](references/xxd-panel-117-prompt.en.md)／[中国語](references/xxd-panel-117-prompt.zh-CN.md)を参照してください。

<!-- xxd-readme-ads:start -->
## XXD について

XXD は Xiaoxiaodong のブランド名略称です。本プロジェクトの作成・管理：[@xiaoxiaodong01](https://x.com/xiaoxiaodong01)。

## Xiaoxiaodong マルチプラットフォーム会員 · 年額 CNY 699

> **広告表示：** 以下のQRコード、会員および有料サービスのリンクはXXDの広告情報です。スキャンや購入は任意であり、オープンソースの利用には影響しません。

年額会員ひとつで、**Knowledge Planet＋XXD会員プロンプトライブラリ＋すべてのGeneral Skills会員**の3つを利用できます。別々に購入する必要はありません。

<!-- xxd-panel-command-system:start -->

### Skills の連携方法

| 区分 | 含まれるもの | 役割 |
|---|---|---|
| **General** | [`xxd-panel-all`](https://github.com/xiaoxiaodong-ai/xxd-panel-all) | 利用可能な番号付きSkillsを検出し、画像・テーマ・用途から推薦し、複数スタイルや一括タスクを整理します。 |
| **Soldier** | `xxd-panel-NNN` | 各番号が固有の原文プロンプトと美学に従い、Generalから割り当てられた具体的な作業を完成させます。 |

<!-- xxd-panel-command-system:end -->

### 会員の内容

1. **XiaoxiaodongをAI学習の相談相手に**
   [Knowledge Planet](https://wx.zsxq.com/group/15554814142882)で、AI学習、ツール、実際のプロジェクトについていつでも質問できます。回答や役立つ内容を会員向けに整理していきます。
2. **継続更新する会員プロンプトライブラリ**
   [XXD会員プロンプトライブラリ](https://vip.xiaoxiaodong.ai/)には現在約3.2万件のプロンプトがあり、10万件超を目標に継続して拡充します。
3. **すべてのGeneral Skillsと利用サポート**
   ひとつの会員で全General Skillsを利用でき、使い方に困ったときは案内やQ&Aを受けられます。
4. **必要性の高い要望を優先**
   会員から寄せられた頻度と必要性の高いプロンプトやSkillsは、優先して検討・開発します。

### 開設方法

- [会員サイトから自分で開設](https://vip.xiaoxiaodong.ai/)できます。
- または下のQRコードからXiaoxiaodongに連絡し、開設を依頼できます。

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="Xiaoxiaodongへの連絡" width="280"></a></p>
<!-- xxd-readme-ads:end -->

## ライセンス

本プロジェクト（Skill、プロンプト、スクリプト、文書、付属サンプル画像を含む）は **PolyForm Noncommercial License 1.0.0** の下で提供されます。完全な法的条文は [LICENSE](LICENSE)、公式ページは <https://polyformproject.org/licenses/noncommercial/1.0.0> を参照してください。

分かりやすく言うと：

- 個人は学習、研究、実験、テスト、趣味のプロジェクト、私的娯楽に使用できます。慈善団体、教育機関、公的研究・安全・保健機関、環境保護団体、政府機関も使用できます。
- **非商業目的**であれば、使用、複製、変更、派生物の作成、共有が可能です。共有時には本ライセンス（または上記リンク）と、作者が示したすべての `Required Notice:` 文を添付する必要があります。
- 商用製品・サービス、有料納品、アクセス権やライセンスの販売、商業利用につながることが予想される用途には使用できません。商用利用には著作権者から別途書面による許可を得てください。
- 本契約が付与するのは明記された著作権ライセンスと限定的な特許ライセンスだけです。商標、ブランド名、その他明記されていない権利は付与されず、ライセンスを第三者へ再許諾することもできません。
- 書面で違反通知を受けた場合、32 日以内に遵守状態へ戻り、実際の是正措置を取らなければライセンスは直ちに終了します。特許侵害を書面で主張した場合も特許ライセンスが終了します。
- 内容は法律が認める範囲で「現状のまま」提供され、保証はありません。利用に伴うリスクと損失は利用者が負います。
