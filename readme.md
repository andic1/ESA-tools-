# OneBox 工具箱 · 一站式在线工具集

<div align="center">

[![OneBox Tools](https://img.shields.io/badge/OneBox-%E5%9C%A8%E7%BA%BF%E5%B7%A5%E5%85%B7%E7%AE%B1-6366f1?style=for-the-badge)](./)
[![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)](LICENSE)

**基于阿里云 ESA Pages 打造的边缘 HTML 工具集：静态页面 + 边缘函数 + 边缘存储 + 缓存**

</div>

---

## 1. 项目简介

OneBox 工具箱 起源于开源项目 JustHTMLs，在其基础上进行了大规模改造，定位为一个 **无需注册、开箱即用、不涉及隐私的一站式在线工具箱**，同时也可作为边缘/静态站点技术实践的示例项目：

- 静态站点托管（可部署在 GitHub Pages、阿里云 ESA Pages 等）
- 边缘函数或轻量服务（统计、排行、推荐等 API）
- 边缘存储 / KV（PV/UV 计数、用户行为）
- 缓存策略（工具索引缓存、统计接口短缓存）

项目形式仍然是「**纯 HTML 工具站**」，但在此基础上加入了 **统计与推荐能力**，让它不仅是一个工具集合，更像是一个围绕实用场景打造的在线工具工作台。

### 1.1 设计理念

- **单文件工具**：所有实际工具仍然是独立的单文件 HTML（内联 CSS/JS），便于复制、二次分发和离线使用。
- **零构建成本**：主站使用原生 HTML/CSS/JavaScript，无需打包构建工具，适合在任何静态托管环境运行。
- **隐私友好**：工具数据默认在浏览器本地处理，统计只记录匿名 ID，不采集个人敏感信息。
- **边缘优先**：PV/UV 统计、工具使用排行、推荐列表等全部在边缘函数上完成，贴近用户侧，降低延迟。
- **缓存友好**：工具索引 `index.json` 和静态资源尽可能长时间缓存，统计与排行接口使用秒级短缓存，兼顾实时性与性能。

---

## 2. 评审维度对应说明

### 2.1 创意性

- 将传统「工具导航站」升级为「基于边缘能力的开发者工作台」，既有实际生产力，又具备展示性。
- 利用边缘统计做出 **工具热度排行、个性化推荐、我的工作台（最近使用 / 收藏）** 等特性，而不引入复杂后端框架。

### 2.2 应用性

- 面向日常前端 / 后端 / 运维工作中常见的小需求：格式转换、文本处理、图片处理、调试工具等，随开即用。
- 通过 PV/UV 统计和排行，可以真实反映哪些工具在团队或社区中最常用，指导优化和推广。

### 2.3 技术探索

- 演示如何在 ESA Pages 上同时使用：静态页面托管 + 边缘函数 + 边缘 KV/存储 + 缓存策略。
- 通过边缘函数实现接近实时的 PV/UV 统计、排行聚合与匿名用户行为记录，构建一个轻量的「边缘分析」能力。

---

## 3. 工具分类

| 分类 | 描述 | 工具数量 |
|------|------|----------|
| 格式转换 | 各种文件和数据格式之间的转换工具 | - |
| 开发者工具 | 面向开发者的实用工具集合 | - |
| 文本处理 | 文本编辑、格式化和处理工具 | - |
| 图片处理 | 图片编辑、转换和优化工具 | - |
| 实用工具 | 日常生活中的实用小工具 | - |

---

## 4. 工具清单

### 格式转换
- Base32 编码
- Base32 解码
- Base36 编码
- Base36 解码
- Base58 编码
- Base58 解码
- Base64 URL 安全编码
- Base64 URL 安全解码
- Base64 编码解码
- CSV 转 JSON
- CSV 转 TSV
- CSV 转 YAML
- HEX 编码
- HEX 解码
- HTML 实体编码/解码
- JSON 字符串转义
- JSON 格式化工具
- JSON 转 CSV
- JSON 转 TSV
- JSON 转 XML
- JSON 转 YAML
- JSONL 转换器
- TSV 转 CSV
- TSV 转 JSON
- URL 编码解码
- Unix 时间戳转换
- XML 转 JSON
- XML 转 YAML
- YAML 转 CSV
- YAML 转 JSON
- YAML 转 XML
- YAML 验证器
- 进制转换工具

### 开发者工具
- CSS 压缩/格式化工具
- Cron 表达式生成器
- Gitignore 生成器
- HTML 压缩器
- HTML 格式化工具
- HTTP 状态码查询
- JSON 压缩器
- JSON 键名排序
- JWT 生成器
- JWT 解码器
- JavaScript 压缩器
- JavaScript 格式化工具
- Meta 标签生成器
- NanoID 生成器
- Robots.txt 生成器
- SQL 压缩器
- SQL 格式化工具
- Sitemap 生成器
- ULID 生成器
- URL 参数生成器
- URL 解析器
- UUID 生成器
- XML 压缩器
- XML 格式化工具
- YAML 压缩器
- YAML 格式化工具
- 哈希生成器
- 正则表达式测试器
- 渐变色生成器
- 颜色对比度检测
- 颜色选择器

### 文本处理
- Emoji 清理器
- 每日一言
- HTML 转 Markdown
- HTML 转纯文本
- JSON 转 Markdown 表格
- Lorem Ipsum 生成器
- Markdown 表格生成器
- Markdown 转 HTML
- Markdown 转纯文本
- ROT13 编码
- URL Slug 生成器
- Unicode 反转义
- Unicode 转义
- 二进制转文本
- 凯撒密码
- 大小写转换工具
- 字数统计工具
- 摩斯电码编码
- 摩斯电码解码
- 文本分割器
- 文本去重工具
- 文本反转工具
- 文本合并器
- 文本对比工具
- 文本换行器
- 文本排序工具
- 文本查找替换
- 文本清理器
- 文本缩进工具
- 文本转 HTML
- 文本转二进制
- 行号添加器
- 行尾符转换器

### 图片处理
- 图片加水印
- 图片压缩工具
- 图片尺寸调整
- 图片拼接
- 图片旋转翻转
- 图片滤镜
- 图片裁剪
- 图片转 Base64
- 图片转 WebP

### 实用工具
- BMI 计算器
- 倒计时器
- 二维码生成器
- 单位换算器
- 字节大小转换器
- 抽签工具
- 掷骰子工具
- 石头剪刀布
- 安全密码生成器
- 密码强度检测
- 日期差值计算器
- 百分比计算器
- 随机抽取器
- 随机数生成器

---

## 5. 快速开始

### 5.1 本地预览

```bash
# 进入项目目录
cd html-tools

# 使用任意静态服务器运行
python -m http.server 8000
# 或者
npx serve .
```

然后在浏览器中访问 `http://localhost:8000` 即可查看首页和全部工具。

> 说明：本地预览时，PV/UV 统计接口 `/api/clicks` 可能不可用，需在部署到 ESA Pages 并绑定对应边缘函数后才会生效。

### 5.2 部署到阿里云 ESA Pages（思路）

> 具体部署命令和控制台配置以赛事官方文档为准，这里只描述架构思路，方便评审理解：

- 将当前仓库作为 **Pages 静态站点** 部署，根目录即为 `html-tools/`。
- 新建一个或多个 **边缘函数**，将 `workers/clicks.js` 中的逻辑迁移到 ESA 的函数运行时：
  - 暴露 `/api/clicks` GET/POST 接口
  - 将 `env.CLICKS_KV` 映射为 ESA 提供的 KV / 表格存储服务
- 在 Pages 路由规则中，将 `/api/*` 前缀转发到对应的边缘函数。
- 在 ESA 提供的边缘缓存能力中：
  - 为 `index.json` 配置较长缓存时间
  - 为 `/api/clicks`、排行等 API 配置短缓存（例如 30–60 秒）。

---

## 6. 工具规范（沿用原 JustHTMLs 约定）

每个工具推荐仍然保持以下结构，方便复用与扩展：

```
tools/
  └── your-tool/
      ├── index.html    # 工具详情页（介绍页面）
      └── app.html      # 工具实体页（实际运行的工具）
```

**设计原则：**

- 单文件 HTML，内联 CSS/JS
- 不使用需要构建的技术栈（如 React/JSX 等）
- 第三方库优先从本地 `assets/vendor` 加载，可选 CDN 兜底
- 保持精简（建议单文件不超过 ~500 行）
- 数据本地处理，保护隐私

如需自定义或新增工具，可以参考 `index.json` 中已有条目的结构进行扩展。

---

## 7. 项目结构

```
html-tools/
├── index.html              # 主站门户首页
├── index.json              # 工具索引文件
├── CONTRIBUTING.md          # 贡献指南
├── README.md               # 项目说明
├── tools/                  # 工具目录
│   └── tool-name/         # 单个工具文件夹
│       ├── index.html     # 工具详情页
│       └── app.html       # 工具实体页
└── .github/
    └── ISSUE_TEMPLATE/    # GitHub Issue 模板
        ├── tool-submission.md
        └── bug-report.md
```

---

## 8. 开发路线图

- [x] 基础网站框架
- [x] 工具索引系统
- [x] 搜索和过滤功能
- [x] 工具提交流程
- [ ] 用户系统（收藏、历史记录）
- [ ] 工具评分和评论
- [ ] 私人工具侧载功能
- [ ] 移动端优化

---

## 9. 技术栈

- **纯 HTML/CSS/JavaScript**：无构建步骤，适合静态托管
- **阿里云 ESA Pages**：预期托管本项目的静态资源与边缘函数
- **边缘 KV / 存储服务（待接入）**：持久化 PV/UV、匿名用户行为等

---

## 10. 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

---

## 11. 鸣谢

- 原项目 [justhtmls/html-tools](https://github.com/justhtmls/html-tools) 及其所有贡献者
- 所有在边缘开发领域分享经验的开发者同行

