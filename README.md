#サンプルデータETLパイプライン

#処理内容
- Googleドライブ上の、エクセル・CSVデータ収集（os, chardet, pandas）
- CSVの、文字エンコード変換（pathlib, unicodedata）
- 収集データの、属性付与・粒度統一・正規化・一時保存（re, SQLite, ”:memory:”）
- 収集データの、統合（変数名：clean_df）
- 統合データ保存①（Googleスプレッドシート）
- 統合データ保存②（.dbファイル）
- 統合データ保存③（BigQuery）

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
