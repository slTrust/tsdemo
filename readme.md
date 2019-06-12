### 环境配置

- node
- npm

#### 安装node

- [node官网download lts版本即可](https://nodejs.org/en/download/)

一路next

验证安装是否成功

```
node -v
npm -v
```

### 安装 ts环境

```
npm install typescript@2.9.2 -g
```

> 安装 ts-node 让 node 支持 ts

```
npm install ts-node@7.0.0 -g
```

#### 1.建立你的代码目录

```
# 到桌面
cd ~/Desktop

# 创建目录
mkdir tsdemo

# 进入目录
cd tsdemo
```

#### 2.创建 tsdemo/.vscode/launch.json

```
{
    "configurations": [
        {
        "name": "ts-node",
        "type": "node",
        "request": "launch",
        "program": "注意看这里，要写成ts-node对应的可执行文件，Windows 用户注意了，你应该写成 ${workspaceRoot}/node_modules/ts-node/dist/bin.js",
        "args": ["${relativeFile}"],
        "cwd": "${workspaceRoot}",
        "protocol": "inspector"
        }
    ]
}
# which ts-node 得到 ts-node命令的路径填入即可
```

#### 3.当前目录新建 1.ts

```
console.log(1);
```

![](https://raw.githubusercontent.com/slTrust/note/master/typescript/ts001-02.png)

![](https://raw.githubusercontent.com/slTrust/note/master/typescript/ts001-03.png)


#### 这样你就配置好了ts所需的环境

#### 开始ts学习

- [5分钟上手](https://www.tslang.cn/docs/handbook/typescript-in-5-minutes.html)
- [doc](https://www.typescriptlang.org/)
- [文档](https://www.tslang.cn/)



