# 国内镜像方案

## 目标

让无法稳定访问 GitHub 的用户也能下载 Skill。

## 当前镜像

第一版国内镜像部署在：

- `https://superbxr.com/downloads/cg-open-skills/`

该镜像是静态下载页，不新增账号系统，不收集用户数据。

## 推荐实现

先做静态页，不做账号系统。

```text
/cg-open-skills/
├── index.html
├── downloads/
│   ├── cg-open-skills-v0.1.1.zip
│   └── single/
├── manifest.json
└── changelog.html
```

## 更新流程

1. 本地生成 zip。
2. 上传到国内静态镜像目录。
3. 更新 `manifest.json`。
4. 飞书文档同步最新下载链接。

## 不做的事

- 不做登录。
- 不做在线编辑。
- 不做自动安装器。
- 不做用户数据收集。
