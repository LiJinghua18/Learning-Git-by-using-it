# 本地Repository与github上的Repository同步的两种方式

- 使用git clone命令
- 使用git remote命令

## 使用git clone命令

**git clone[repository地址(可以是http地址，也可以是ssh地址)]**

该命令将从远程下载一个仓库到本地，之后本地有任何更新都可以直接使用git add、git commit、git push命令进行上传更新

## 使用git remote命令

使用本命令有两个前提条件：

- **本地**已经有了 git 仓库A（新建仓库使用git init命令）

- **远程**也有了一个 git 仓库B（如果是github，请参照github上新建仓库的方法）

  要想A与B关联，在仓库A下执行git命令**git remote add origin [B地址(可以是http地址，也可以是ssh地址)]**，执行成功后，本地有任何更新都可以直接使用git add、git commit、git push命令进行上传更新。

