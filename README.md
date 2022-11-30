# 脚本执行管理
----
# 感谢猫猫提供技术支持
----

## 开发须知

###### `如何在自己的脚本中引用软件的获取的Cookie？`

```js
console.log(process.env.APP_COOKIE)
```

###### 在开发中你也要避免变量重复 APP_COOKIE 这是默认必传的

----

  #### 需要安装Node js

  https://baidu.com

  #### 切换 npm 源

  `npm config set registry https://registry.npm.taobao.org/`

#### 需要执行 

  `npm install` 

#### 运行

  `node file.js`

#### 配置 

##### 库中的 config.json 文件是脚本的配置文件

``` js
{
    "name": "测试脚本",  // 脚本的名称（随便写 给展示的）
    "file": "test",  // 对应仓库中的文件名不包含后缀 (test.js)
    "version": "1",  // 这是版本 更新后改动这里
    "cron": "0 */2 * * * *", // 定时任务默认的配置
    "env": [
        {
            "envName": "xjhd", // 环境变量 比如你脚本中是 process.env.xjhd 
            "envHint": "习酒Token多个用@隔开" // 变量描述
        }
    ],
    "scope": "" // 如果是空就  京 了 美 三个都显示  如果跟包名 则对应显示  详情参考模板库
}
```



#### 仓库配置

![image](https://m.360buyimg.com/babel/jfs/t1/211099/2/29105/154108/63863510E74633584/c80a350901a54c39.png)

#### 效果图

![image](https://m.360buyimg.com/babel/jfs/t1/75794/34/22715/137844/636d9bf6Eee52ad72/c02b0754a3b4ae95.jpg)
![image](https://m.360buyimg.com/babel/jfs/t1/91605/37/32751/122090/636d9beeE2224ba57/9c4ca62297ba7d2e.jpg)
