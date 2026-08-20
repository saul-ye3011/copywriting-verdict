# Copywriting Verdict / 文案大师

这是「文案大师」的可安装与可共创发行包。

## 包含内容

- `versions/00-original-prompt.md`：最早的「小丰」角色提示词。
- `versions/01-copywriting-verdict/`：当前完整 skill，包括主规则、参考框架与评测用例。
- `dist/copywriting-verdict.skill`：可直接安装的 skill 压缩包。
- `VERSION_HISTORY.md`：已确认的版本沿革与来源说明。

## 安装

将 `dist/copywriting-verdict.skill` 导入支持 `.skill` 的 Codex/Claude skill 管理器，或解压 `versions/01-copywriting-verdict/` 到 skills 目录。

## 共创

通过 GitHub Pull Request 修改 `versions/01-copywriting-verdict/`。请保持五维文案裁决框架为核心，新增执行规则时同步补充 `evals/evals.json`，并在 `VERSION_HISTORY.md` 记录变化。

## 权限说明

本包适合放在 GitHub private repository。GitHub 私有仓库只有获授权的协作者能通过链接访问、安装和提交修改。

