# High Quality Web Frontend Agent

Portable Codex skill for building, reviewing, and improving polished web frontends. Entry point: `SKILL.md`.

## Importing this skill

A Codex skill is imported by copying the whole skill folder into the Codex skills directory. The important part is that `SKILL.md` must be directly inside the imported folder.

### 1. Choose the target skills directory

Use `$CODEX_HOME/skills` when `CODEX_HOME` is set. If it is not set, use the default Codex home directory:

```sh
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
```

### 2. Copy this repository into that directory

From the parent directory of this repository, run:

```sh
cp -R high-quality-web-frontend-agent "${CODEX_HOME:-$HOME/.codex}/skills/high-quality-web-frontend-agent"
```

If you are already inside this repository, run:

```sh
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills/high-quality-web-frontend-agent"
cp -R . "${CODEX_HOME:-$HOME/.codex}/skills/high-quality-web-frontend-agent"
```

### 3. Verify the folder layout

After copying, this file must exist:

```text
${CODEX_HOME:-$HOME/.codex}/skills/high-quality-web-frontend-agent/SKILL.md
```

### 4. Reload Codex

Start a new Codex session, or reload skills if your environment supports it. Codex discovers the skill from the YAML frontmatter at the top of `SKILL.md`.

## 日本語での手順

1. このリポジトリのフォルダごと Codex の skills ディレクトリにコピーします。
2. コピー後に `.../skills/high-quality-web-frontend-agent/SKILL.md` という配置になっていることを確認します。
3. Codex を再起動、またはスキルを再読み込みします。
4. フロントエンド UI の品質改善、レスポンシブ対応、アクセシビリティ、見た目の polish に関する依頼で自動的に使われます。

## Troubleshooting

- If the skill does not appear, check that the file is named exactly `SKILL.md`.
- If the skill still does not trigger, confirm that the folder containing `SKILL.md` is directly under the skills directory.
- If you copied from inside the repository, avoid accidentally creating a nested path such as `skills/high-quality-web-frontend-agent/high-quality-web-frontend-agent/SKILL.md`.
