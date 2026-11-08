[English](README.md) | [日本語](README.ja.md)

<p align="center">
  <img src="./assets/blueprint-header.ja.svg" alt="sora：建築の法規から、エージェントのハーネスへ。一級建築士・一級建築施工管理技士。AIコーディングエージェントのハーネス・MCPサーバー・オーケストレーションを作っています。" width="100%">
</p>

<p align="center">
  <a href="https://x.com/sora_biz"><img src="https://img.shields.io/badge/X-@sora__biz-1D3E6B?style=for-the-badge&labelColor=14324F&logo=x&logoColor=white" alt="X"></a>
  <a href="https://sorabiz.substack.com/"><img src="https://img.shields.io/badge/Substack-連載を読む-1D3E6B?style=for-the-badge&labelColor=14324F&logo=substack&logoColor=white" alt="Substack"></a>
  <a href="https://zenn.dev/sora_biz"><img src="https://img.shields.io/badge/Zenn-記事一覧-1D3E6B?style=for-the-badge&labelColor=14324F&logo=zenn&logoColor=white" alt="Zenn"></a>
</p>

<h2><img src="./assets/section-notes.svg" alt="01 General Notes" width="100%"></h2>

1. **AI コーディングエージェントのハーネスとガードレール**を設計しています。Claude Code / Codex / Windows でのマルチエージェント運用が中心です。
2. **専門領域 × AI。** 一級建築士・一級建築施工管理技士として、建築基準法や宅建業法を AI が幻覚しないための法令 MCP サーバーを作っています。
3. **Windows ネイティブな開発体験**を重視しています。エージェントツールの多くは Unix 前提なので、そこを埋めるツールを作っています。
4. **執筆。** AI コーディングの実践を [Substack](https://sorabiz.substack.com/) と [Zenn](https://zenn.dev/sora_biz) で連載しています。

<h2><img src="./assets/section-works.svg" alt="02 Schedule of Works" width="100%"></h2>

| 記号 | プロジェクト | 仕様 | 材料 |
|:---:|---|---|---|
| `W‑1` | [**winsmux**](https://github.com/Sora-bluesky/winsmux) | エージェント間通信のための Windows ネイティブなターミナルマルチプレクサ。WSL なしで tmux 的なオーケストレーション | Rust |
| `W‑2` | [**kbd-signal**](https://github.com/Sora-bluesky/kbd-signal) | VIA 対応キーボードの RGB で Claude Code / Codex セッションの状態を表示するステータスランプ | Python |
| `S‑1` | [**building-standards-act-mcp**](https://github.com/Sora-bluesky/building-standards-act-mcp) | e-Gov API 連携の建築基準法 MCP サーバー。条文を一次情報で照合し、AI の幻覚を防ぐ | TypeScript |
| `W‑3` | [**security-loop**](https://github.com/Sora-bluesky/security-loop) | Windows PC と VPS に入っているバージョンを OSV・ランタイムの勧告・CISA KEV と照合する。影響の判定はスキャンのたびに確かめ直す | Python |
| `T‑1` | [**x-jimaku**](https://github.com/Sora-bluesky/x-jimaku) | x.com の動画にリアルタイムで日本語字幕を重ねる Chrome 拡張。ローカル Whisper (WebGPU) と Chrome 内蔵の翻訳 API で動く | TypeScript |
| `T‑2` | [**checkchart**](https://github.com/Sora-bluesky/checkchart) | フローチャート・シーケンス図・構成図を、Mermaid で描く前に事実と読みやすさの面で確かめる | TypeScript |

<h2><img src="./assets/section-tools.svg" alt="03 Tools on Site" width="100%"></h2>

<p>
  <img src="https://img.shields.io/badge/Claude%20Code-1D3E6B?style=for-the-badge&logo=anthropic&logoColor=white" alt="Claude Code">
  <img src="https://img.shields.io/badge/Codex-1D3E6B?style=for-the-badge&logoColor=white&logo=data:image/svg%2Bxml;base64,PHN2ZyBmaWxsPSJ3aGl0ZSIgcm9sZT0iaW1nIiB2aWV3Qm94PSIwIDAgMjQgMjQiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHRpdGxlPk9wZW5BSTwvdGl0bGU+PHBhdGggZD0iTTIyLjI4MTkgOS44MjExYTUuOTg0NyA1Ljk4NDcgMCAwIDAtLjUxNTctNC45MTA4IDYuMDQ2MiA2LjA0NjIgMCAwIDAtNi41MDk4LTIuOUE2LjA2NTEgNi4wNjUxIDAgMCAwIDQuOTgwNyA0LjE4MThhNS45ODQ3IDUuOTg0NyAwIDAgMC0zLjk5NzcgMi45IDYuMDQ2MiA2LjA0NjIgMCAwIDAgLjc0MjcgNy4wOTY2IDUuOTggNS45OCAwIDAgMCAuNTExIDQuOTEwNyA2LjA1MSA2LjA1MSAwIDAgMCA2LjUxNDYgMi45MDAxQTUuOTg0NyA1Ljk4NDcgMCAwIDAgMTMuMjU5OSAyNGE2LjA1NTcgNi4wNTU3IDAgMCAwIDUuNzcxOC00LjIwNTggNS45ODk0IDUuOTg5NCAwIDAgMCAzLjk5NzctMi45MDAxIDYuMDU1NyA2LjA1NTcgMCAwIDAtLjc0NzUtNy4wNzI5em0tOS4wMjIgMTIuNjA4MWE0LjQ3NTUgNC40NzU1IDAgMCAxLTIuODc2NC0xLjA0MDhsLjE0MTktLjA4MDQgNC43NzgzLTIuNzU4MmEuNzk0OC43OTQ4IDAgMCAwIC4zOTI3LS42ODEzdi02LjczNjlsMi4wMiAxLjE2ODZhLjA3MS4wNzEgMCAwIDEgLjAzOC4wNTJ2NS41ODI2YTQuNTA0IDQuNTA0IDAgMCAxLTQuNDk0NSA0LjQ5NDR6bS05LjY2MDctNC4xMjU0YTQuNDcwOCA0LjQ3MDggMCAwIDEtLjUzNDYtMy4wMTM3bC4xNDIuMDg1MiA0Ljc4MyAyLjc1ODJhLjc3MTIuNzcxMiAwIDAgMCAuNzgwNiAwbDUuODQyOC0zLjM2ODV2Mi4zMzI0YS4wODA0LjA4MDQgMCAwIDEtLjAzMzIuMDYxNUw5Ljc0IDE5Ljk1MDJhNC40OTkyIDQuNDk5MiAwIDAgMS02LjE0MDgtMS42NDY0ek0yLjM0MDggNy44OTU2YTQuNDg1IDQuNDg1IDAgMCAxIDIuMzY1NS0xLjk3MjhWMTEuNmEuNzY2NC43NjY0IDAgMCAwIC4zODc5LjY3NjVsNS44MTQ0IDMuMzU0My0yLjAyMDEgMS4xNjg1YS4wNzU3LjA3NTcgMCAwIDEtLjA3MSAwbC00LjgzMDMtMi43ODY1QTQuNTA0IDQuNTA0IDAgMCAxIDIuMzQwOCA3Ljg3MnptMTYuNTk2MyAzLjg1NThMMTMuMTAzOCA4LjM2NCAxNS4xMTkyIDcuMmEuMDc1Ny4wNzU3IDAgMCAxIC4wNzEgMGw0LjgzMDMgMi43OTEzYTQuNDk0NCA0LjQ5NDQgMCAwIDEtLjY3NjUgOC4xMDQydi01LjY3NzJhLjc5Ljc5IDAgMCAwLS40MDctLjY2N3ptMi4wMTA3LTMuMDIzMWwtLjE0Mi0uMDg1Mi00Ljc3MzUtMi43ODE4YS43NzU5Ljc3NTkgMCAwIDAtLjc4NTQgMEw5LjQwOSA5LjIyOTdWNi44OTc0YS4wNjYyLjA2NjIgMCAwIDEgLjAyODQtLjA2MTVsNC44MzAzLTIuNzg2NmE0LjQ5OTIgNC40OTkyIDAgMCAxIDYuNjgwMiA0LjY2ek04LjMwNjUgMTIuODYzbC0yLjAyLTEuMTYzOGEuMDgwNC4wODA0IDAgMCAxLS4wMzgtLjA1NjdWNi4wNzQyYTQuNDk5MiA0LjQ5OTIgMCAwIDEgNy4zNzU3LTMuNDUzN2wtLjE0Mi4wODA1TDguNzA0IDUuNDU5YS43OTQ4Ljc5NDggMCAwIDAtLjM5MjcuNjgxM3ptMS4wOTc2LTIuMzY1NGwyLjYwMi0xLjQ5OTggMi42MDY5IDEuNDk5OHYyLjk5OTRsLTIuNTk3NCAxLjQ5OTctMi42MDY3LTEuNDk5N1oiLz48L3N2Zz4=" alt="Codex">
  <img src="https://img.shields.io/badge/Grok%20Build-1D3E6B?style=for-the-badge&logo=x&logoColor=white" alt="Grok Build">
  <img src="https://img.shields.io/badge/Antigravity-1D3E6B?style=for-the-badge&logo=google&logoColor=white" alt="Antigravity">
  <img src="https://img.shields.io/badge/MCP-1D3E6B?style=for-the-badge&logo=modelcontextprotocol&logoColor=white" alt="MCP">
</p>
<p>
  <img src="https://img.shields.io/badge/Rust-1D3E6B?style=for-the-badge&logo=rust&logoColor=white" alt="Rust">
  <img src="https://img.shields.io/badge/TypeScript-1D3E6B?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Python-1D3E6B?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/PowerShell-1D3E6B?style=for-the-badge&logo=gnometerminal&logoColor=white" alt="PowerShell">
  <img src="https://img.shields.io/badge/JavaScript-1D3E6B?style=for-the-badge&logo=javascript&logoColor=white" alt="JavaScript">
</p>

<h2><img src="./assets/section-record.svg" alt="04 Site Record" width="100%"></h2>

<p align="center">
  <img src="./assets/stats.svg" alt="GitHub stats" height="165">
  <img src="./assets/top-langs.svg" alt="Top languages" height="165">
</p>

<h2><img src="./assets/section-writing.svg" alt="05 Specifications: Writing" width="100%"></h2>

- [WSLなしでWindowsにtmuxを：Rust製psmuxでペイン分割とAIエージェント並列実行](https://zenn.dev/sora_biz/articles/psmux-windows-native-tmux)
- [Hermes Agent完全構築ガイド｜VPSに常駐する自分専用AIエージェントの作り方](https://zenn.dev/sora_biz/articles/hermes-vps-complete-guide)
- [【第13回】メモを自分で探すな。Hermes AgentはObsidianを記憶として読む](https://zenn.dev/sora_biz/articles/hermes-vps-13-obsidian)

ほかの記事は [Zenn](https://zenn.dev/sora_biz)（全記事 `?locale=en` で英語版あり）と [Substack](https://sorabiz.substack.com/) へ。

<p align="center"><img src="./assets/title-block.svg" alt="Title block: Sora-bluesky, drawn by sora, sheet 1 of 1" width="100%"></p>

<p align="center">
  <a href="https://x.com/sora_biz">X</a> の DM を開けています。AI エージェントのツール、Windows の開発体験、建築 × AI の話を歓迎します。
</p>
