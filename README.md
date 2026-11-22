# 场景拼音 · 数字电路版

基于 Rime/雾凇拼音的 Windows 拼音输入方案，面向数字电路课程学习场景。
在 Windows 小狼毫（Weasel）上使用。

## 特性

1. **场景词库切换**：`通用拼音`（日常）与 `数字电路`（专业词库）两个方案，`Ctrl+\`` 或 `F4` 一键切换
2. **相邻键纠错**：数字电路场景下，输入 `huogei`（f/g 相邻键误按）也能打出「或非」
3. **场景独立词频**：两个方案的用户词频分别记在各自的 userdb，互不干扰
4. **低门槛部署**：下载 zip → 解压 → 双击 `一键部署.bat` 即完成

## 快速开始

1. 安装小狼毫：https://github.com/rime/weasel/releases
2. 从右侧 **Releases** 下载最新 zip，解压到任意目录
3. 双击 `一键部署.bat`（自动备份现有配置 → 复制 → 重新部署）
4. 切换到「小狼毫」输入法，`Ctrl+\`` 选择「通用拼音」或「数字电路」

## 加你自己的词

四个接口，详见 zip 内 `README使用说明.md`：

| 接口 | 说明 |
|---|---|
| 自动记忆 | 选词即学，userdb 独立积累 |
| `custom_phrase.txt` | 一行 `词<Tab>编码` 置顶，推荐 |
| `digital_circuit.dict.yaml` | 直接编辑专业词库（词/权重） |
| `import_tables` | 新建词库文件后挂一行即合并 |

## 致谢

- 词库与方案基于 [雾凇拼音 rime-ice](https://github.com/iDvel/rime-ice)（GPL-3.0）
- Rime 输入法框架：[librime](https://github.com/rime/librime) · [小狼毫 Weasel](https://github.com/rime/weasel)
