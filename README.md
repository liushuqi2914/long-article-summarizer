# 长文章总结概括（long-article-summarizer）

一个用于**长文章（尤其是学术论文、研究报告）结构化总结**的 WorkBuddy 技能（Skill）。

## 它能做什么

把一篇长文章快速提炼为：

- **一句话概括（TL;DR）** —— 一句话说清"做了什么 + 结论"
- **分层摘要** —— L1 极简 / L2 标准 / L3 详细，三档字数递进
- **结构化要点** —— 研究问题与背景 / 方法与数据 / 主要发现 / 结论与贡献 / 局限与展望

## 触发方式

只要在对话里说"总结 / 概括 / 提炼 / 归纳 / 摘要 / 这篇讲了什么 / 核心观点"，就会自动触发本技能。

## 支持的输入方式

| 方式 | 示例 |
|------|------|
| 直接粘贴文本 | 「总结一下：」+ 粘贴全文 |
| 本地文件 | 「总结 `D:\论文\xxx.pdf`」（支持 docx / pdf / txt / md） |
| 网页链接 | 「总结这个链接 https://...」 |

## 目录结构

```
long-article-summarizer/
├── SKILL.md                          # 技能定义（总结工作流 + 输出模板）
└── references/
    └── academic-summarization.md     # 学术论文总结详细指南
```

## 安装方法

### 方式一：放入用户级 skills 目录

1. 下载本仓库（或 `long-article-summarizer.zip`）。
2. 将 `long-article-summarizer` 文件夹复制到：

   - **Windows**: `C:\Users\<你的用户名>\.workbuddy\skills\`
   - **macOS / Linux**: `~/.workbuddy/skills/`

3. 重启 WorkBuddy（或新建对话），即可生效。

### 方式二：通过技能市场安装（若已发布）

在 WorkBuddy 左侧菜单【专家·技能·连接器】→【技能】→【技能市场】中搜索「长文章总结概括」并安装。

## 使用示例

> 用户：总结一下这篇文章 https://zhuanlan.zhihu.com/p/333386099

技能会输出：

```
## 一句话概括
...

## 分层摘要
**L1 极简：** ...
**L2 标准：** ...
**L3 详细：** ...

## 结构化要点
### 研究问题与背景
...
```

## 许可

[MIT License](LICENSE)
