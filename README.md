# YZSpecs

## YZSpecs 是什么

>YZSpecs 是作者的个人私有仓库。

## specs 用到的命令总结：

#### 制作本地库
> 
* 打开目录，cd到指定目录，输入指令创建库。“YZUtils”是库的名字。
* 创建本地库<pre><code>pod lib create YZUtils</code></pre>
* 先在自己GitHub账户下新建一个YZUtils库来存放代码
* 添加远程地址<pre><code> git remote add origin https://github.com/zone1026/YZUtils.git </code></pre>
* 提交到master分支 <pre><code> git push -u origin master </code></pre>
* 新建tag <pre><code>git tag 0.1.0 </code></pre>
* 提交tag 0.1.0 <pre><code>git push origin 0.1.0 </code></pre>

#### 提交到官方的CocoaPods
> 
* 校验 .podspec文件 <pre><code>pod lib lint --allow-warnings </code></pre>
* 如果没有注册pod账号，请执行 <pre><code>pod trunk register EMAIL [NAME] </code></pre>
* 提交到cocoapods <pre><code>pod trunk push YZUtils.podspec --allow-warnings </code></pre>

#### 提交到自己私有的Specs上
<p>
> 
* 先在GitHub账户下公开的创建spec库 <pre><code>https://github.com/zone1026/YZSpecs.git </code></pre>
* 添加本地specs库 <pre><code>pod repo add YZSpecs https://github.com/zone1026/YZSpecs.git </code></pre>
* 把YZUtils.podspec推送到YZSpecs库中 <pre><code>pod repo push YZSpecs YZUtils.podspec --allow-warnings </code></pre>
* 查看我们本地的Specs库：打开Findle，Shift+Command+G -> 前往文件夹 -> 输入：~/.cocoapods/repos ->点击前往，就可以看到YZSpecs文件夹，与master同级
>
## HYZNetwork 是什么

>HYZNetwork 是基于 [AFNetworking][AFNetworking] 封装的iOS端简易网络库，通过创建请求对象的方式处理网络接口.

## YZUtils 是什么
>YZUtils是项目开发过程中用到的一些工具类，总结归纳，方便后期开发。

## 联系方式

>zone1026, 1024105345@qq.com

