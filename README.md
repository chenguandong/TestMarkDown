# TestMarkDown
[TOC]
#1.0用户登陆
## 1.1 用户登陆
请求格式
```
请求格式
{
	"cmd":"register"

	"param":{
	"nickName":"马云",              //用户姓名
	"company":"淘宝",               // 单位名称
	"phone": "18539902139",    //手机号码
	"password": "123123123", // 密码  (注意移动端MD5加密后传给服务器)
	}
}

```
返回格式
```
{
“result”:”0”    //0 成功 1 失败
“resultNote”:”失败原因”
“userInfo”:

{
	  “UID”:”12”,                         //用户ID

	“nickName”:”马云”,                 //用户姓名
	“company”:”淘宝”,                   // 单位名称
	“phone”: “18539902139”,         //手机号码
	“vipLevel” :  “1”   ,              // 1 普通用户   2 vip 用户 3 VIP已缴费没有上
	传资料 4 vip 已经交费 资料审核中  5 vip 已经交费资料审核没有通过
	“userNum”: “12345” ,         //用户编号(3-5 位)
	“userIcon”: “http://xxx.png” //用户头像
}


}
```
