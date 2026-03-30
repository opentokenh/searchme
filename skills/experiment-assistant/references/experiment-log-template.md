# Experiment Log Template

## 文件路径
`research/experiments/YYYY-MM-DD-[slug].md`

## 完整模板

```markdown
# [实验名称]

## 基本信息
- 日期：YYYY-MM-DD
- 实验目的：
- 假设：

## 配置
- 模型：
- 数据集：
- 关键超参数：
- commit（如使用repo）：
- 运行环境：

## 实验记录
- 第一次运行：结果...
- 调整：...
- 第二次运行：...

## 结果
- 主要指标：[metric] = [value]
- 对比基线：相比[baseline]提升/下降[X%]
- 意外情况：

## 结论
- 是否支持假设？
- 下一步：

## 关联论文
- 参考了哪些论文的方法？
```

## 常用 ML Metrics

| 任务 | Metrics |
|------|---------|
| 分类 | Accuracy, Precision, Recall, F1, AUC-ROC |
| 检测 | mAP, IoU, AP@50, AP@75 |
| 生成 | BLEU, ROUGE, FID, CLIP Score |
| 多模态 | VQA Accuracy, ChartQA, TextVQA |
| Agent | Success Rate, Task Completion |
