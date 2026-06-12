# LLM-prompting-bestpractice (prompt optimizer)

外部 LLM サービスに投入するプロンプトを **3 ベンダー統合 best practice**（Anthropic / OpenAI / Edison
Scientific）で設計・最適化する Claude Code Skill。XML タグ構造化・5 コンポーネント（role / task / context /
format / constraints）・outcome-first 指示・Anti-pattern 検査を整合的に適用します。

研究者向け LLM ツール（**Edison Scientific Kosmos / Elicit / Perplexity / ChatGPT / Claude.ai**）への投入に
特化。特に Kosmos のような**実行中に修正できない長時間自律型**への single-objective 設計に対応します。

## いつ使うか
- 外部 LLM に投げる prompt を新規作成 / レビュー / 別ベンダーへ移植する。
- 別マシン・自律実行用の agentic prompt を作る（anti-hallucination ガード付き）。
- `/LLM-prompting-bestpractice` で起動、または「このプロンプトを最適化して」等。

逆に、いま対話している Claude Code セッションへのその場の通常 prompt には不要です。

## インストール
```sh
git clone https://github.com/eUmeda/LLM-prompting-bestpractice.git
ln -s "$PWD/LLM-prompting-bestpractice" ~/.claude/skills/LLM-prompting-bestpractice
```

## 出典
Anthropic / OpenAI / Edison Scientific の**公開** best practice ドキュメント、および arXiv
（2305.13062 / 2312.16171 / 2309.11495 / 2406.06608 ほか）に基づき、出典 URL は `SKILL.md` 内に明記。
本 Skill は各社原則を**統合・蒸留した二次的著作物**であり、原典の**実質的な逐語転載は含みません**（短い引用は出典付きで使用）。

## 利用上の注意（Terms / Disclaimer）
現状有姿（**AS IS**）・無保証。**利用は自己責任**で。出力プロンプトの品質や外部 LLM の挙動について作者は
責任を負いません。

## 引用（Citation）
役立った場合、引用やリンクでの言及を歓迎します（必須ではありません）。
> Eisaku Umeda (2026). *LLM-prompting-bestpractice*. https://github.com/eUmeda/LLM-prompting-bestpractice

## License
MIT — see [LICENSE](LICENSE).

---
🤖 Built and maintained with [Claude Code](https://claude.com/claude-code).
