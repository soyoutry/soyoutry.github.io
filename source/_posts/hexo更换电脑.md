---
title: 使用Hexo更换了电脑，如何重新部署
---



- 安装git

```text
sudo apt-get install git
```

- 设置git全局邮箱和用户名

```text
git config --global user.name "yourgithubname"
git config --global user.email "yourgithubemail"
```

- 安装nodejs

- 安装hexo  

  ```
  cnpm install
  ```

但是已经不需要初始化了，

直接在任意文件夹下，

```text
git clone git@………………
```

然后进入克隆到的文件夹：

```text
cd xxx.github.io
npm install
npm install hexo-deployer-git --save
```

生成，部署：

```text
hexo g
hexo d
```



然后就可以开始写你的新博客了

```text
hexo new newpage
```



**Tips:**

1. 不要忘了，每次写完最好都把源文件上传一下

```text
git add .
git commit –m "xxxx"
git push 
```

1. 如果是在已经编辑过的电脑上，已经有clone文件夹了，那么，每次只要和远端同步一下就行了

```text
git pull
```