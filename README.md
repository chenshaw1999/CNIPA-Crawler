# CNIPA-Crawler

## 1. Introduction

A web crawler based on Selenium

## 2. Installation

### 2.1. Dependencies

* FirefoxDriver (Already placed in repo)
* Selenium

### 2.2. A CNIPA account

You must have a account before run this web crawler

And you can create a account from [here](http://pss-system.cnipa.gov.cn/sipopublicsearch/portal/uiregister-showRegisterPage.shtml, 'link')
```python
driver = get_driver(username = "", password = "")
```

### 2.2. Usage

```python
get_table(driver, 0, "CN102340805B")
```

The crawler will search from "热门工具 >> 引证/被引证查询 >> 引证"

And get the table of grant number "CN102340805B" like ->
				

GrantNo | id | 相关性 | 公开号 | IPC分类号 | 相关段落 | 相关权利要求 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| CN102340805B | 0| A | CN101141184A | H04B7/005; H04Q7/34; H04B7/26 |  |  |
| CN102340805B | 0|  | CN101141184A | H04B7/005; H04Q7/34; H04B7/26 |  |  |
 ...
| CN102340805B | 0 | Y | US2010027510A1 |  |  |  |
| CN102340805B | 0 |  | US2010027510A1 |  |  |  |
| CN102340805B | 0 |  |  |  |  |  |
