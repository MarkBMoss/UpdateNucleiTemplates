# Nuclei Poc 全网收集
UpdateNucleiTemplates，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei Templates，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2026-09-30 19:53`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 108868 | cve | 63916 | medium | 44055 |
| 2 | wordpress | 103126 | other | 54765 | low | 39760 |
| 3 | wp-plugin | 95199 | wordpress | 5924 | high | 27615 |
| 4 | low | 37671 | auth | 4666 | info | 26025 |
| 5 | medium | 35251 | sql | 3998 | critical | 15949 |
| 6 | candidate | 34243 | detect | 2498 | unknown | 149 |
| 7 | production | 18156 | microsoft | 2410 | informative | 17 |
| 8 | high | 17426 | remote_code_execution | 1993 | hight | 16 |
| 9 | tech | 17281 | web | 1308 | meduim | 13 |
| 10 | detect | 16392 | social | 1237 | cretical | 4 |

**81 个目录，44572 个文件**
## 如何使用

### 克隆项目

克隆这个项目到本地：

```bash
git clone https://github.com/MarkBMoss/UpdateNucleiTemplates.git
```

进入项目目录：

```bash
cd UpdateNucleiTemplates
```

### 配置

在 `repo.txt` 文件中配置监控 GitHub 项目信息。

### 运行脚本

运行 Python 脚本：

```bash
python UpdateNucleiTemplates.py
```

### GitHub Action

在 GitHub 仓库中设置 Action，以便每日自动运行脚本。

> 需要配置`Workflow permissions`为`Read and write`权限

## 文件结构

- `NucleiPocGather.py`: 收集全网 Nuclei POC 的脚本文件。
- `DeWeight.py`: 对现有的 Nuclei POC 进行进一步去重的脚本文件。
- `WirteREADME.py`: 统计现有的 POC 并更新 README.md 文件。
- `repo.txt`: Nuclei POC 仓库列表。
- `poc.txt`: 已存档 POC 列表。
- `poc/`: 存放分类后的 Nuclei POC 文件夹。
- `原始仓库`：`https://github.com/lianqingsec/NucleiPocGather`
- 添加了部分`Nuclei Poc Templates`仓库，主要自用并优化该项目。
