# Host-scan
### RongScan中的host碰撞板块，Rongscan还在内测中，先将部分模块进行放出
### 用于发现内网才可以访问的系统
<br>
<br>
<br>

## 功能支持
### 1. 常见内网域名字典的生成 
### 2. 自定义异步线程
### 3. 状态码显示
![image](https://github.com/FFR66/host-scan/assets/110553194/d7d8c1b5-3bfa-4e48-a138-9dde0dc18f6c)
<br>
<br>
<br>

## 如何使用
### 将发现40x的url，放在url.txt中，将收集到的domain全部放在host.txt中
  Rongscan_HostScan.exe -uf .\urls.txt -hf .\hosts.txt -o fkalis.txt
  <br>
   
  ![image](https://github.com/FFR66/host-scan/assets/110553194/d3ca7366-15f9-4e9d-8e91-c12782dd3919)



<br>
<br>
<br>

## host内网域名自定义（主要用于常见的内网域名）
<br>

### %domain% --> 会自动变为当前host中的全部根域名
#### 例如：admin.%domain% 规则
**如果host.txt中存在www.baidu.com 和 www.csdn.com**
**其在进行爆破的时候会自动变为admin.baidu.com 和 admin.csdn.com**
<br>
<br>
<br>


## 使用案例


**运行输出格式为 [+] {status} {url} {host}  -->  {content_length} : {title}**
![image](https://github.com/FFR66/host-scan/assets/110553194/1027f1f3-5359-4f6a-946c-60e33d91c254)

<br>

**成功案例**
![image](https://github.com/FFR66/host-scan/assets/110553194/c9a47f3e-ac85-4113-bd56-e9c0e77ceee3)



<br>
<br>
<br>




## 致谢
### 如果各位师傅觉得写的还可以的，麻烦点一个star，欢迎各位师傅提交pr，我们共同进步！！
### 如果想要参与rongscan内测的，师傅可以联系我。


<br>
<br>
<br>

## bug
### 第一版自定义线程有bug，报错就使用第二版，非常抱歉！
