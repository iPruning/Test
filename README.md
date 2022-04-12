# 某某书

- [某某书](#某某书)
  - [README](#readme)
    - [项目目标](#项目目标)
    - [项目节奏](#项目节奏)
    - [作品展示](#作品展示)
  - [绝对坐标](#绝对坐标)
    - [信息流动图](#信息流动图)
  - [相关工具](#相关工具)
    - [安装 mdbook](#安装-mdbook)
    - [启动 mdbook 网站](#启动-mdbook-网站)
    - [编译 HTML、PDF、Word](#编译-htmlpdfword)
  - [ChangeLog](#changelog)

## README

### 项目目标

### 项目节奏

- `*wd*` #TODO
- `*wd*` #TODO

### 作品展示

最终呈现在 [main Branch](https://github.com/<替换为你的仓库路径>/tree/main)，方式待未定，可能以 Web 作品呈现。

## 绝对坐标

| 实体 | 功能 | 绝对坐标 |
|---|---|---|
| `.github/` | 存放 GitHub 的配置，如 Issue 模版、Pull Request 模版、Action 机器人等。 | [🔗](.github/) |
| `book/` | 存放电子书的编译文件，由 mdbook 生成，不上传到 GitHub 里。 | [🔗](book/) |
| `docs/` | 存放会议纪要等文档。 | [🔗](docs/) |
| `src/` | 存放书籍的源文件。 | [🔗](src/) |
| `book.toml` | 是 mdbook 的配置文件，用于编译书籍。 | [🔗](book.toml) |
| `README` | 是项目的唯一入口。 | [🔗](README.md) |

### 信息流动图

```txt
微信群/私下会议/独立探索/ ... 任何即时场景中
        ^ \
        |  +- 触发创想/改进点/卡片创意/读书疑问点/...
        |   \               
        |    *- => Issues 进行具体描述/追踪/讨论/...
        ^   / \         +- https://github.com/<替换为你的仓库路径>/issues
        |   |  \            +- 自动提醒 -> #TODO 需要配置
        |   ^   +- 定期 腾讯会议/飞书会议 交流嗯哼
        |   |   |       +- #TODO 需补充会议号
        |   ^   +- 定期 Master Branch 发布周任务 (*wd0 2042)
        |   |   |       +- https://github.com/<替换为你的仓库路径>/tree/master
        ^   ^   +- 笔记 追踪在 https://github.com/<你的 Fork 的仓库路径>
        |   |   |     +- 小伙伴专有 Fork 仓库中
        |   |   |         +- 提交规格 Commit Message 
        |   |   |             +- 含对应 Issue 标号
        |   |   |            /
        |   +---+-----<---<-+ (将自动匹配增补到对应 Issue 时间线事件中)
        |       |       
        ^       +- 知识点/经验/手册 沉淀到 Wiki 在完全配置之前暂放于 Master Branch 
        |      /      +- https://github.com/<替换为你的仓库路径>/wiki
        +---<-+       +- https://github.com/<替换为你的仓库路径>/tree/master
```

## 相关工具

### 安装 mdbook

```shell
brew install mdbook
cargo install mdbook-pdf
cargo install mdbook-linkcheck
asdf reshim
```

### 启动 mdbook 网站

```shell
mdbook serve --open
```

### 编译 HTML、PDF、Word

```shell
mdbook build
```

## ChangeLog

- XXXX-XX-XX init

<p xmlns:cc="http://creativecommons.org/ns#" >This work is licensed under <a href="http://creativecommons.org/licenses/by-nd/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-ND 4.0
