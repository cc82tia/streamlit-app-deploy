~/CodeLogs/                    ← すべての学習・試行ログの親ディレクトリ
├── streamlit/                ← 技術ごとのサブフォルダ
│   ├── 2025-07-25_form-trial/
│   │   ├── app.py            ← コード
│   │   ├── v1_fail.py        ← 途中失敗作（分けて残すと学習になる）
│   │   ├── v3_success.py     ← 成功版
│   │   └── README.md         ← ログ・メモ（コメント欄代わり）
│   └── summary.md            ← Streamlit全体の学びまとめ
├── langchain/
│   ├── 2025-07-20_retriever-agent/
│   │   ├── agent.py
│   │   └── README.md
│   └── summary.md
├── errors/
│   ├── AttributeError_log.md
│   ├── FileNotFound_log.md
│   └── summary.md
└── overall_summary.md        ← 技術横断での振り返りまとめ


# 📝 2025-07-25 Form入力の状態管理

## 👩‍💻 試したこと
- v1_fail.py：st.form_submit_button() の後に状態反映されなかった
- v3_success.py：callbackでstateを更新 → 成功！

## 💬 コメント
- 一瞬うまくいったと思ったが再実行時にstateが飛ぶ罠があった
- session_stateはやはり「辞書のように初期化して使う」が正解

## 🔎 キーワード
form, session_state, callback, streamlit, state管理

## 📁 関連ファイル
- `v1_fail.py`
- `v3_success.py`
