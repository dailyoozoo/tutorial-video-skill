# tutorial-video skill

把操作截图打包成完整解说视频的自动化 skill：截图 → 解说词 → TTS 配音 → karaoke 字幕 → 背景音乐 → 封装，全流程带防坑约束与阶段 QC。

沉淀自一次真实生产（AWS 教程 v1-v8，2026-10-10）：9 条泛化约束、9 个历史教训、完整 QC 清单，全部内建，开箱即用。

## 结构

- `SKILL.md` — 主流程（7 步管线 + 文字/断句规则）
- `references/constraints.md` — 9 条通用约束（C1-C9）
- `references/lessons.md` — v1-v8 历史教训 → 约束映射
- `references/qc-checklist.md` — 阶段门禁 + 终检清单
- `references/pronunciation.md` — 多音字审计指南

## 核心约束速览

| 编号 | 约束 | 来源 |
|---|---|---|
| C3 | 音频 acrossfade 必须与视频 xfade 一一对应 | v5 2.4s 漂移 |
| C8 | 终检必须跑成品文件，禁纸面 QC | v6 扫描盲区 |
| C2 | karaoke 时长零重分配 | v5 高亮错位 |
| C9 | 先出完整问题清单再动手 | 挤牙膏修复 |
