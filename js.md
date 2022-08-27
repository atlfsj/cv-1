准备工作
```
yarn global add parcel@1.12.3       //安装版本
parcel src/index.html               //将index.html的相对路径放在parcel后将会启动服务器                
parcel会自动刷新
```

细节
```
let n = 1;
dmeo.innerHTML = n;
let step = () {
    setTimeout(() => {
        n = n+1;
        demo.innerHTNL = n;
    }, 1000)
};

step();      // 1=>2
step();2000      //不能这么写，因为实效不对
```

正则表达式
```
string = string.replace(/\n/g, "<br>");     //使用正则表达式（/ /g）将回车显示出来，不用则只有第一个回车显示
```

背景渐变 <br>
搜索 css gradient background generator，将色彩设置到50%，左白右黑，中间加一个渐变设置到50%，左白右黑，再将下面的代码复制到你的代码中；<br>
镜像渐变：内外

<br>
dist中的文件是可以直接发布的，scr不可以 
<br>
部署到github之前先安装parcel的旧版本

```
yarn global add parcel@1.9.7
parcel build src/index.html --no-minify --public-url .
```

<br>
一般不提交 .cache文件，放到.gitignore中（最前面加个/表示是最外面的目录）

<br>
当github page不出现预览地址时，多刷新几次或退出重进；打开是404后面要加路径（dist/xxx）

<br>
尽量吧css写外边


