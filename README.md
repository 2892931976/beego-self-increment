
## beego-self-increment
为了解决Beego Orm多条数据循环无法获取自增id的问题,自己写了这个小方法<br>
## 项目地址
github地址: https://github.com/kiwi520/beego-self-increment<br>
欢迎使用并提出不足

## 使用方法
   ### 首先安装此包<br>
    go get  github.com/kiwi520/beego-self-increment
   ### 引用此包
``` go    
    self "github.com/kiwi520/beego-self-increment"
```   
``` go
    var ai *self.AutoInc<br>
    ai = self.New(NumberId,1) //第一个参数你的自增id初始值,第二个参数是自增幅度 比如每次自增1
    for _,v :=range JsonData{
	Ai :=ai.Id() //自增id
        ...
    }
    
```
    
   
   
