# Slash Command: run-roo (Intent Trigger)
# Gemini CLI Definition (Primary)
name = "run-roo"
description = "Roo Code CLI (roo) を使用して自律的なタスクを実行します。"

prompt = """
ユーザーは Roo Code CLI (`roo`) を使用してタスクを実行しようとしています。
以下の引数を解析し、適切な `roo` コマンドを実行してください。

### 引数 ({{args}}) の解析
- `--mode <mode>`: 指定されたモード（architect, code, ask, debug, orchestrator 等）を使用します。デフォルトは "code" です。
- `<prompt>`: タスクの内容です。

### 実行手順
1. **CLI の確認とセットアップ**:
   - `/home/coder/.local/bin/roo` が存在するか確認してください。
   - 存在しない場合は、以下のコマンドでインストールを実行してください。
     ```bash
     /home/coder/project/.infra/scripts/setup_roo.sh
     ```
2. **環境変数の確認**:
   - `OPENROUTER_API_KEY` または `ANTHROPIC_API_KEY` が設定されているか確認してください。
3. **コマンドの実行**:
   - 以下の形式で `roo` CLI を実行してください。モデルはユーザー指定がなければ `minimax/minimax-m2.1:free` を使用します。
     ```bash
     /home/coder/.local/bin/roo --mode "<mode>" --model "minimax/minimax-m2.1:free" --print "<prompt>"
     ```
4. **結果の解析と報告**:
   - 実行結果を取得し、タスクの完了状態や出力をユーザーに報告してください。
"""
