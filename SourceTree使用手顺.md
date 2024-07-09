# SourceTree使用手顺

## 0. 前言

Sourcetree是一款开源的Git客户端，功能强大且易于使用。本文将介绍Sourcetree的安装、配置、常用操作和参考资料。

## 1. 下载安装

1.1.  下载地址：https://www.sourcetreeapp.com/
![图片](https://github.com/moerbumo/kilig/blob/94f23d0cdb8c77e4dc66982f992cdba88d7dbacb/image.png?raw=true)
1.2.1. 安装：跳过登录项。
![图片](https://github.com/moerbumo/kilig/blob/614b753345d5d493b4f35511bdaeb3b3d9ddcf3e/%E5%AE%89%E8%A3%851.png?raw=true)
1.2.2. 选择安装路径，若未安装过Git，请先安装Git。点击`下一步`继续。
![图片](https://github.com/moerbumo/kilig/blob/438c276b89f14e3d857a08f1d5c333165ee67791/%E5%AE%89%E8%A3%852.png?raw=true)
1.2.3. 程序会自动读取git配置信息，点击`下一步`完成安装。
![图片](https://github.com/moerbumo/kilig/blob/438c276b89f14e3d857a08f1d5c333165ee67791/%E5%AE%89%E8%A3%853.png?raw=true)

## 2. 克隆仓库

### 2.1.  URL克隆：使用URL或SSH地址克隆仓库。

- 克隆SSH地址：选中要克隆的项目，点击右上角的的 `Switch to SSH` 按钮，复制SSH地址。
    - 若SSH地址不存在，请先配置SSH公钥到OneDev。
    - 1. 打开`Git Bash`, 输入命令 `ssh-keygen -t rsa` 生成SSH密钥，三次回车生成id_rsa和id_rsa.pub文件，默认在C:\Users\用户名\.ssh目录下。
    - 2. 打开OneDev，点击左侧导航栏中的`SSH Keys` -> `New SSH Key` ，将id_rsa.pub文件内容粘贴到`Key`输入框。
    - 3. 复制SSH地址，点击菜单栏中的`Repository` -> `Clone Repository` -> `Clone with SSH` 克隆仓库。
- 克隆HTTP地址：选中要克隆的项目，点击右上角的的 `Clone with HTTP` 按钮，复制HTTP地址。
   - 1. 打开Sourcetree，点击菜单栏中的`文件` -> `克隆仓库` 克隆仓库，下面可以选择本地仓库的存储位置。
    ![图片](https://github.com/moerbumo/kilig/blob/39db5fdd9372ce6c285fba28eaee8407583452b5/01.png?raw=true)
    - 2. 新建分支用于开发，点击远程，选中main分支右键，选择`检出`。
    ![图片](https://github.com/moerbumo/kilig/blob/39db5fdd9372ce6c285fba28eaee8407583452b5/02.png?raw=true)
   - 3. 在本地确定分支名称。
    ![图片](https://github.com/moerbumo/kilig/blob/39db5fdd9372ce6c285fba28eaee8407583452b5/03.png?raw=true)
   - 4. 本地进行开发修改，将修改结果提交到本地仓库。
    ![图片](https://github.com/moerbumo/kilig/blob/39db5fdd9372ce6c285fba28eaee8407583452b5/04.png?raw=true)
   - 5. 将结果提交到develop分支，在OneDev上进行pull request,合并确认。
    ![图片](https://github.com/moerbumo/kilig/blob/39db5fdd9372ce6c285fba28eaee8407583452b5/05.png?raw=true)
   - 6. 点击导航栏中的`pull requests`，新增一个pull request。
    ![图片](https://github.com/moerbumo/kilig/blob/39db5fdd9372ce6c285fba28eaee8407583452b5/06.png?raw=true)
  - 7. 确认develop分支修改信息，没有问题点击下方的合并分支按钮。
    ![图片](https://github.com/moerbumo/kilig/blob/39db5fdd9372ce6c285fba28eaee8407583452b5/07.png?raw=true)
  - 8. 合并完成后，在main分支可以查看到合并结果。
    ![图片](https://github.com/moerbumo/kilig/blob/39db5fdd9372ce6c285fba28eaee8407583452b5/08.png?raw=true)

### 2.2.  本地克隆：将本地仓库克隆到Sourcetree。

- 1. 打开Sourcetree，点击菜单栏中的`文件` -> `克隆仓库` 克隆仓库，下面可以选择本地仓库的存储位置，或者直接点击右上方加号，选择`Add`。
    ![图片](https://github.com/moerbumo/kilig/blob/b06bb79cde6b1abc67761851910b5eac36c9eff8/09.png?raw=true)

- 2. 后续操作同上。

## 3. 常用操作

- 克隆仓库：点击菜单栏中的`Repository` -> `Clone Repository`
- 推送代码：点击菜单栏中的`Repository` -> `Push`
- 拉取代码：点击菜单栏中的`Repository` -> `Pull`
- 创建分支：点击菜单栏中的`Repository` -> `Branch` -> `New Branch`
- 切换分支：点击菜单栏中的`Repository` -> `Branch` -> `Switch Branch`
- 合并分支：点击菜单栏中的`Repository` -> `Branch` -> `Merge`
- 解决冲突：点击菜单栏中的`Repository` -> `Resolve Conflicts`
- 标签管理：点击菜单栏中的`Repository` -> `Tags`
- 版本管理：点击菜单栏中的`Repository` -> `Commits`
- 日志查看：点击菜单栏中的`Repository` -> `Log`
- 远程仓库管理：点击菜单栏中的`Repository` -> `Remotes`
- 忽略文件：点击菜单栏中的`Repository` -> `Ignore`

## 4. 参考资料

- [Sourcetree 使用手顺](https://www.cnblogs.com/protosoft/p/11286592.html)
- [Sourcetree 常用操作](https://blog.csdn.net/GM_115/article/details/133188369)
- [git 版本管理](https://blog.csdn.net/qq_52748334/article/details/137019947)
