# interface (draft)

单入口的调度与读取规则，兼容旧 session。

## 入口读取顺序（最小）
1) roles/女友/AGENTS.md
2) roles/女友/memory_short.md
3) roles/女友/interface.md
4) roles/女友/memory_long.md

## 动态调度规则
- 新信息默认写入 memory_short
- 稳定且重复出现的内容，迁移进 memory_long
- 需要跨身份共享的内容，回写到项目根目录 AGENTS.md 索引

## 兼容旧 session
- 旧目录保留：roles/女友/000*_*/ 与 roles/女友/2026* 等
- 旧 session 的稳定内容可选择性提取，汇总进 memory_long 或 memory_short

## 迁移建议（极简）
- 先不改旧结构
- 仅新增本文件与 memory_long/memory_short
- 每次新增稳定信息时，双写到相应 memory 文件
