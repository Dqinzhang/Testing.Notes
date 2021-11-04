#### 版本管理工具 Git

##### 1.Git 是什么

Git 可以对文档资料进行共享，管理及权限控制

> Git：是一个==开源==的==分布式==版本控制系统,可以有效,高速的处理从很小到很大的项目版本管理。
>
> * GitHub：全球最大的面向开源及私有软件项目的托管平台。
>
> > 是一个基于 Git 实现的在线代码托管仓库。
>
> * GitLab：类似于 GitHub ，但 GitLab 可以部署在服务器上，通常用于企业团队内部协作开发。
>
> > 是一个基于 Git 实现的在线代码仓库软件。



##### 2.Git 的使用

* Git Clone克隆

*一个项目仅需要克隆 1 次*

> 登录 GitHub
>
> 点击右上角头像
>
> 点击 `Your repositories`
>
> 点击 `New` 创建新的存储库

![创建新的存储库](https://i.loli.net/2021/11/04/PgBYuN6kJAvQewS.png)

![输入仓库相关信息](https://i.loli.net/2021/11/04/njEhPpW5yk7bZod.png)

---

> 点击新建的项目
>
> 点击 `Code`
>
> 点击 `SSH`
>
> 点击 复制

![克隆远程仓库](https://i.loli.net/2021/11/04/ekExBwlG2WpOitD.png)

> 进入本地仓库
>
> 空白处鼠标右键菜单选择 `Git 克隆`
>
> 粘贴上一步复制的`SSH`
>
> 加载存储在本地的私钥

![Git克隆](https://i.loli.net/2021/11/04/PxfEyHRtBMA7TFG.png)

![Git克隆_02](https://i.loli.net/2021/11/04/j4xIMaKbhpvfZN5.png)

---

* Git 从远程仓库拉取文件到本地仓库

> 进入本地仓库
>
> 空白处鼠标右键菜单选择 `TortoiseGit`
>
> 点击 `拉取`

![从远程仓库拉取文件到本地仓库](https://i.loli.net/2021/11/04/4aCkux5TSOLzobm.png)



* Git 从本地上传文件到远程仓库

> 首先将需要上传的文件移动到本地仓库
>
> 空白处鼠标右键菜单选择 `TortoiseGit`
>
> 选择`添加`

![image-20211104130053476](https://i.loli.net/2021/11/04/fHhEZSJx7Q9C51P.png)

![image-20211104130212749](https://i.loli.net/2021/11/04/FWJmUiBbnKosqVG.png)

![image-20211104130311089](https://i.loli.net/2021/11/04/WDfRa1QTbMNq6K5.png)

![image-20211104130608133](https://i.loli.net/2021/11/04/6saHtXrJxjOz38p.png)

> 点击 `提交`

![image-20211104130713876](https://i.loli.net/2021/11/04/KcMQ68ausxJz1CS.png)

> 点击 `推送`

---

* Git 删除文件

> 首先在本地仓库将需要删除的文件 Delete
>
> 鼠标右键菜单选择 `Git 提交`
>
> 填写日志信息后点击 `提交并推送`

![image-20211104134854475](https://i.loli.net/2021/11/04/FOCYUmrH7aRZebq.png)

![image-20211104134905438](https://i.loli.net/2021/11/04/rjf8VcNdAew7EyS.png)



* Git 还原

*ps：前提是删除的文件未提交*

> 空白处鼠标右键菜单选择 `TortoiseGit`
>
> 选择 `还原`

![image-20211104135302156](https://i.loli.net/2021/11/04/CfkMnDIsm5iAlUd.png)

> 选择需要还原的文件
>
> 点击 `确定`

![image-20211104135556653](https://i.loli.net/2021/11/04/7srtLVhgJl25Oie.png)



---

##### 3.Git 与 SVN 的区别

* SVN 版本集中管理，所有代码都在一天服务器上；分支和主线是不一样的URL地址路径
* Git 分布式管理，去中心化，服务器和每个开发人员都拥有一个本地的代码管理仓库；分支和主线路径是一样的
