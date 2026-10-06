# SSD 学习平台 - 超级紧凑 Prompt

## 一句话说明
用 React + Vite 构建一个从零到一的 SSD 学习应用，包含 5 个学习阶段、SMART 监控、性能测试、故障诊断、可视化仪表盘。

## 核心需求

### 技术栈
React + Vite + TypeScript + Tailwind CSS + React Router + Recharts

### 5 个学习阶段（Chapter）
1. **SSD 基础** - NAND/控制器/磨损均衡/TRIM/over-provisioning
2. **SMART 监控** - SMART 属性/健康评估/故障预测
3. **性能测试** - 顺序读写/随机读写/IOPS/延迟/队列深度
4. **故障诊断** - 寿命下降/温度高/掉盘/性能下降/坏块增加
5. **可视化监控** - SSD 仪表盘/温度趋势/写入量/健康状态

### 主要页面
- **首页 Dashboard** - 学习进度、章节卡片、推荐路径、学习统计
- **章节页** - 左侧导航 + 右侧内容、知识点卡片、学习目标
- **课程详情** - 定义/原理/案例/术语/注意事项、"继续学习"按钮
- **SMART 参数** - 参数表格、含义/影响/正常范围/风险、可视化
- **性能测试** - 测试指标说明、读写曲线、场景对比
- **故障诊断** - 故障类型、排查流程、SMART 告警、checklist
- **可视化仪表盘** - 温度/写入/读取/健康/容量趋势图
- **测验页** - 选择题/判断题、解析、正确率统计
- **个人中心** - 学习进度、打卡、推荐下一节

### 数据模型
```
Chapter {id, title, description, order, progress, difficulty, status}
Lesson {id, chapterId, title, content, keyPoints, duration, completed}
SmartMetric {id, name, meaning, riskLevel, normalRange, unit, category}
Quiz {id, chapterId, type, question, options, answer, explanation}
Stats {totalChapters, completedLessons, accuracyRate, ...}
```

### 关键特性
- ✅ 学习进度条、章节完成打勾
- ✅ "标记已读"、快速切换下一节
- ✅ 深色/浅色模式
- ✅ 响应式设计
- ✅ Mock 数据（不需要后端）
- ✅ 图表展示（Recharts）
- ✅ 卡片化布局
- ✅ 清晰的信息层级

### 配色
科技蓝/青色主题 - 适合 SSD/系统监控风格

### 输出
- 完整可运行的 React 项目
- 清晰的目录结构
- 主要页面组件代码
- Mock 数据文件
- 路由配置
- 样式文件
- README（中文）
- 无需后端，前端可完整演示

---

**核心要点：这是一个教育类学习平台，需要清晰的内容组织、视觉上易于理解、支持完整学习闭环。**
