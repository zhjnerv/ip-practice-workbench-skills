# 公开发布准备

## 当前状态

本目录已作为私有 GitHub 仓库 [zhjnerv/ip-practice-workbench-skills](https://github.com/zhjnerv/ip-practice-workbench-skills) 推送，默认分支为 `main`，首次提交为 `d9022fb`。仓库当前保持私有；未创建公开远端，也未声明任何线上入口已经随本次更新。

## 公开内容

根 README、MIT LICENSE、维护说明、验证脚本与三个技能目录组成候选。每个技能包含独立 LICENSE 和 NOTICE，供单独安装时一并保留。

`.local/`、根 TASK_PLAN、运行缓存、下载产物和环境变量文件由 [.gitignore](../.gitignore) 排除。发布时核对实际 Git 清单，不复制整个原工作区。

## 尚需完成的发布事项

1. 审阅 [MIT 文件](../LICENSE) 和 [数据、模板来源范围](../DATA_SOURCES.md)。确认需要公开的数据包及其权利依据；当前本地迁移没有补齐来源证据的事实。
2. 在确认数据再分发范围和用户对公开性的明确选择后，将 `zhjnerv/ip-practice-workbench-skills` 转为公开仓库，或按确认后的范围调整发布内容。
3. 公开后核对公开页面、安装说明、默认分支与仓库内容。
4. 发布成功后处理 `myskill` 移除与入口替换；如需要门户新增开源入口，再同步门户源文件与发布目录。

## 验证入口

```bash
python -B -S -X utf8 scripts/verify.py
```

实际验收结果记录于 [迁移记录](migration.md)。离线测试不替代数据来源审查或联网能力验证。
