#サンプルデータETLパイプライン

#処理内容
- Googleドライブ上の、エクセル・CSVファイルの走査・収集（os, chardet, pandas）
- CSVの、文字エンコード変換（pathlib, unicodedata）
- 収集データの抜粋、要・不要列の抜粋（不要だが加工する見出し列名は”中間列_〇〇”として保存）
- 属性の付与、粒度の統一、正規化、インメモリ一時保存（re, SQLite, :memory:）
- 収集データの、統合（変数名：clean_df）
- 統合データ保存①（Googleスプレッドシート編）
- 統合データ保存②（.dbファイル編）
- 統合データ保存③（BigQuery編）
- （率や割合といった係数指標はBIツール内で計算する想定）

#フォルダー構造
sample-data-etl.git/

  ├ README.md

  ├ data-raw/

    └ 2026-01/

      └ sample-data-202601.csv

    └ 2026-02/

      └ sample-data-202602.csv

    └ 2026-03/

      └ sample-data-202603.xlsx

  └ notebooks/

      └ sample-data-etl.ipynb
