# Nuclei Poc 全网收集
UpdateNucleiTemplates，每日更新

这个项目是一个 Python 脚本，用于批量克隆 GitHub 项目，获取 Nuclei Templates，并将 POC 按类别分类存放到文件夹中。同时，使用 GitHub Action 每日自动运行脚本。
# POC 详情统计

> **当前项目 POC 更新时间：**`2025-07-06 14:56`

| ID | 标签      | 数量 | 目录       | 数量 | 严重性   | 数量 |
|:---| :-------- | :--- | :--------- | :--- | :------- | :--- |
| 1 | cve | 40073 | cve | 33995 | medium | 21979 |
| 2 | wordpress | 35793 | other | 26432 | info | 19373 |
| 3 | wp-plugin | 33269 | auth | 2510 | high | 13494 |
| 4 | medium | 15793 | wordpress | 1497 | low | 10247 |
| 5 | tech | 13656 | detect | 1342 | critical | 7406 |
| 6 | detect | 12861 | remote_code_execution | 875 | unknown | 91 |
| 7 | service | 11679 | microsoft | 723 | informative | 17 |
| 8 | low | 9018 | web | 698 | hight | 16 |
| 9 | high | 6229 | sql | 616 | meduim | 6 |
| 10 | http | 4358 | api | 595 | cretical | 2 |

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
