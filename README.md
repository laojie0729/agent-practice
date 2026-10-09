# Agent Practice

用于 DevFlow AI 的 Issue、PR 和 CI 练习的小型 Python 项目。
不依赖额外 Python 包。

## 本地测试

```bash
python3 -m unittest discover -v
```

## 练习

1. 创建 Issue：支持浮点数相加，并补充测试。
2. 创建分支 `practice/float-add`，修改类型标注并增加测试，然后提交 PR。
3. 查看 GitHub Actions，正常结果应为绿色。
4. 在该分支故意把 `return a + b` 改成 `return a - b` 并提交。
5. CI 会因测试失败变红，让 DevFlow AI 分析失败原因及 PR 风险。
6. 恢复加法实现并提交，确认 CI 重新变绿。

GitHub Actions 需要在 GitHub 上运行；本地执行测试不会触发它。
