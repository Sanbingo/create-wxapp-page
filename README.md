# create-wxapp-page

[![Build Status](https://travis-ci.org/cantonjs/create-wxapp-page.svg?branch=master)](https://travis-ci.org/cantonjs/create-wxapp-page)

## 功能

- 自动化生成微信小程序页面，样式支持自定义
- 自动更新`app.json`,添加生成页面
- [NEW]自动化生成微信小程序组件，样式支持自定义
- [NEW]支持自定义模板

## 安装

```bash
$ yarn add create-wxapp-page
```


## 用法

### 查看帮助
```bash
$ create-wxapp-page --help
```

### 创建页面
#### 示例一
（使用yes模式，没有配置的内容使用默认值进行配置）
```bash
$ create-wxapp-page --name test --indent 2 --yes
```

#### 示例二
（不使用yes模式，没有配置的内容，需要通过回答问题，进行配置）
```bash
$ create-wxapp-page --name test
#回答问题
#自动生成...
```

#### 参数
- dir: 文件路径
- name: page的名称，支持带相对/绝对路径(`/path/my-page`, `path/my-page`, `your/path/`, `my-page`)
- type: 创建的页面类型，page，component可选，默认page
- style: 样式文件后缀名，支持 less, scss, wxss 或自定义
- json: 是否需要生成配置文件
- indent: 缩进的方式，默认tab，支持数字
- yes: 使用默认值生成相关文件
- help: 查看帮助

### 重置模板
```bash
$ create-wxapp-page reset
```

### 查看模板位置
```bash
$ create-wxapp-page dir
```

### 打开模板目录
```bash
$ create-wxapp-page open
```


## 自定义模版

1. 通过 `create-wxapp-page open` 命令打开模版目录
2. 编辑并替换默认模版
3. 完成

*Tips* 若需要重置使用默认模版，可以执行 `create-wxapp-page reset` 命令


## 更新日志
[Changelog](/CHANGELOG.md)


## License

MIT
