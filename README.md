# buildadmin第三方登录插件

## 功能特性

1、支持微信、QQ、微博三种登录方式
2、支持账号绑定和新注册登录
3、支持免绑定登录模式
4、支持第三方登录和解绑
5、支持个人资料中心绑定和解绑第三方登录(1.3.0+)

xIzJkQsZTKrbqUBvEShkza35wMGAR1p0mK3Ijg==
使用说明：
1、在使用之前请务必申请对应第三方平台的应用，获得应用ID和应用密钥。
2、微信公众号请使用微信公众号平台登录获取appid和secret填写到第三方登录插件配置中去，然后在微信公众号平台的公众号设置->功能设置->网页授权域名填写你的域名并验证通过。

snsapi_base: 免提示登录，但无法获取用户的昵称、头像等
snsapi_userinfo: 首次需要关注公众号才能登录，但可以获取用户的昵称、头像等信息
各平台密钥申请

微信公众号：(https://mp.weixin.qq.com/)
微信网站应用：(https://open.weixin.qq.com/)
QQ：(https://connect.qq.com/)
微博：(https://open.weibo.com/connect)

回调地址
QQ：`https://www.example.com/third/callback/qq`
微信：`(https://www.example.com/third/callback/wechat`
微博：`https://www.example.com/third/callback/weibo`

常见问题
1、微信中提示app_id不能为空？
请在后台管理插件配置中配置微信公众号的app_id和app_secret

2、微信中使用微信登录提示redirect_uri域名与后台配置不一致，错误码10003？
检查下公众号是否完成认证，必须认证后才可以使用公众号登录功能。
检查下公众号设置与开发->公众号设置->功能设置->网页授权域名配置中的回调域名是否已配置，或是否配置正确。
检查你的公众号类型，微信登录只支持服务号使用

3、微信登录提示AppID不正确？
请前往后台->插件管理->配置微信公众号和微信网站应用的参数
