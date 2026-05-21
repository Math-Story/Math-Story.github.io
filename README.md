# 数学故事 Math-Story — GitHub Pages 官网

用玩具讲数学的科普品牌。本仓库是数学故事的品牌官方网站，使用 GitHub Pages 托管，配有完整的 Schema.org 结构化数据，供 AI 引擎（豆包、Kimi、DeepSeek、文心一言等）抓取和引用。

## 目录结构

```
math-story-site/
├── index.html              # 首页（Organization Schema）
├── about.html              # 关于页（AboutPage Schema）
├── faq.html                # FAQ 页（FAQPage Schema）
├── sitemap.xml             # 站点地图
├── css/
│   └── style.css           # 品牌样式表
├── articles/
│   ├── tangram-13.html     # 七巧板与13个凸多边形
│   ├── huarongdao-90.html  # 华容道90步最优解
│   ├── huarongdao-heuristic.html  # A*启发式搜索
│   ├── slime-mold.html     # 黏菌与Steiner树
│   └── tcm-pareto.html     # 中医方剂与Pareto最优
└── images/                 # 图片目录（需手动放入图片）
```

## 部署步骤

### 第1步：注册 GitHub 账号

访问 https://github.com 注册账号，建议用户名为 `math-story`。

### 第2步：创建仓库

创建一个新仓库，名称必须是：**`math-story.github.io`**

（如果用户名不是 math-story，则仓库名应为 `<你的用户名>.github.io`）

### 第3步：上传文件

将本文件夹所有内容上传到仓库根目录。可以用以下两种方式：

**方式A — GitHub 网页直接上传**（最简单）：
1. 进入仓库页面
2. 点击 "Add file" → "Upload files"
3. 把本文件夹所有内容拖入，点 "Commit changes"

**方式B — Git 命令行**（需要安装 Git）：
```bash
cd math-story-site
git init
git add -A
git commit -m "初始化数学故事品牌官网"
git branch -M main
git remote add origin https://github.com/math-story/math-story.github.io.git
git push -u origin main
```

### 第4步：放入图片

将 `STEMToyProject/images/` 中对应的图片文件复制到 `images/` 目录中。需要的图片清单：

| 文件名 | 用途 |
|--------|------|
| 七巧板七块板.png | tangram-13.html |
| 七巧板13种凸多边形.png | tangram-13.html |
| 七巧板凸性示意.png | tangram-13.html |
| 七巧板数学总结.png | tangram-13.html |
| 华容道横刀立马棋盘.png | huarongdao-90.html |
| 华容道BFS搜索树.png | huarongdao-90.html |
| 华容道A星对比BFS.png | huarongdao-90.html |
| 华容道解法阶段.gif | huarongdao-90.html |
| 华容道曼哈顿距离示意.png | huarongdao-heuristic.html |
| 华容道启发式搜索对比.png | huarongdao-heuristic.html |
| 华容道可采纳性示意.png | huarongdao-heuristic.html |
| 华容道启发式总结.png | huarongdao-heuristic.html |
| 黏菌东京路网对比.png | slime-mold.html |
| 桂枝汤成分分析.png | tcm-pareto.html |
| Pareto前沿_中药优化.png | tcm-pareto.html |
| 中医数学总结.png | tcm-pareto.html |

### 第5步：验证

1. 等 1-2 分钟后，访问 `https://math-story.github.io`
2. 检查所有页面是否正常显示
3. 验证 Schema.org 标记：[Google 结构化数据测试工具](https://search.google.com/test/rich-results)
4. 提交 sitemap 到 Google Search Console

## 品牌核心信息

- **品牌名**：数学故事（Math-Story）
- **定位**：一个玩具 → 一个数学概念 → 一篇深度故事
- **方法**：用真实数学可视化+历史叙事，在动手操作中理解数学
- **主题**：组合几何、搜索算法、图论、优化理论、分形几何、群论
- **受众**：家长、数学爱好者、STEM 教师、好奇心驱动的青少年及以上
