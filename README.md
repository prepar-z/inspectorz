# inspectorz
Java 代码审计 idea 插件
## 介绍
- inspectorz 为 idea 静态代码扫描插件，可一键搜索出所有 sink 点
- 在原有基础上，修改了一些代码逻辑，sink 点更加全面
- 补充添加了多个规则，例如补充了文件读取、文件写入、反序列化等风险点的检测规则，添加了权限绕过、rpc 调用等风险点的检测规则
- 原作者 KimJun
- 原版插件链接
- https://github.com/KimJun1010/inspector

## 安装
- 依次打开
- 设置 -> 插件 -> 本地安装

![image](https://github.com/user-attachments/assets/5688d538-21ab-4585-a650-87204a0ac526)
![image](https://github.com/user-attachments/assets/060805b8-5422-425b-9de9-b83b96d12daa)
![image](https://github.com/user-attachments/assets/29cf6892-93ee-4022-98c2-db3d366da08d)

- 选择下载的 jar 文件即可

## 使用
- 反编译后，右键反编译后的文件夹，进行一键静态扫描

![image](https://github.com/user-attachments/assets/18695fc7-f716-4f50-849c-5ad000c4dce6)
![image](https://github.com/user-attachments/assets/a7d9d50d-8eef-4a9e-a13e-c6e97547ae80)

- 可以把除了插件外的选项都取消勾选

![image](https://github.com/user-attachments/assets/4c0143c0-093f-4d03-a924-0c341adfeec3)

- 配置好后，针对反编译后的文件夹，进行扫描即可

![image](https://github.com/user-attachments/assets/a20f388f-f0bf-43ea-98df-fdb612413bb0)

- 也可根据在人工审计的时候，高亮显示风险点，协助审计
- 例如依据 web.xml 中的配置，跟进后可看到高亮显示的风险点

![image](https://github.com/user-attachments/assets/3c0fcc7d-8e85-4271-b826-67fb3ec0bb3c)
![image](https://github.com/user-attachments/assets/09cc7f34-79c9-422e-8142-5f1cc28dc4ee)


## 优化点
- 在原项目基础上，添加的一些规则
- 例如
- 文件操作类

![image](https://github.com/user-attachments/assets/7faae186-40d0-43df-b5e4-b6327ea706e8)
![image](https://github.com/user-attachments/assets/8534edd0-5cf5-46d1-8eac-0099c9f302e1)

- 权限绕过类

![image](https://github.com/user-attachments/assets/8254abba-ca85-4412-a788-c2feb0580811)
![image](https://github.com/user-attachments/assets/69185f55-7cb4-4a6f-850c-5c01b2e5132a)

- rpc 调用类

![image](https://github.com/user-attachments/assets/5ed57917-ca45-494d-b810-402c8fad046c)
![image](https://github.com/user-attachments/assets/9c194d76-df32-45e3-9710-9ad52504d3d1)

