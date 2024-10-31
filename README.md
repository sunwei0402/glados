# Glados自动签到

## 使用方式：

### 注册一个GLaDOS的账号([注册地址](https://glados.space/landing/M8543-E4N37-Z0JZY-BHTS0)

#### 我的邀请码：([M8543-E4N37-Z0JZY-BHTS0](https://glados.space/landing/M8543-E4N37-Z0JZY-BHTS0)) 

### **Fork**本仓库

![1](https://github.com/user-attachments/assets/a55bc065-9108-4875-9541-96ab4d5e0c9f)


### 添加**secret**

1. 跳转至自己的仓库的`Settings`->`Secrets and variables`->`Action`

2. 添加1个`repository secret`，命名为`COOKIES`，其值对应GLaDOS账号的cookie值中的有效部分（获取方式如下）

- 在GLaDOS的签到页面按`F12`

- 切换到`Network`页面下，刷新

![2](https://github.com/user-attachments/assets/157121fa-868c-490e-8d13-59437ffa41c1)


- 点击第一个选项卡后在`Request Headers`下找到`Cookie`，右键复制cookie的值即可

  > 参考格式：koa:sess=eyJ1c2xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxAwMH0=; koa:sess.sig=xJkOxxxxxxxxxxxxxxxtnM;

![3](https://github.com/user-attachments/assets/11661a99-53b4-4d22-bd32-f8681ae90c04)


- 多账号请在 `COOKIES` 中 添加多个 `cookies` 中间使用 `&`连接即可。（例如： `c1&c3&c3...`）

3. 手机推送（非必须）

- 添加1个`repository secret`，命名为`SENDKEY`，其值对应 PushDeer key: [获取地址]([http://www.pushplus.plus](https://www.pushdeer.com/product.html))。

### **star**自己的仓库

![4](https://github.com/user-attachments/assets/06d75d9c-ab99-4b31-8074-d3dd37b4a10e)


## 文件结构

```shell
│  checkin.py	# 签到脚本
│
├─.github
│  └─workflows
│          gladosCheck.yml	# Actions 配置文件
```

## 声明

本项目不保证稳定运行与更新, 因GitHub相关规定可能会删库, 请注意备份
