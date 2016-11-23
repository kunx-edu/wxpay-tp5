基于thinkphp5的微信扫码支付sdk
===============

[个人博客-御风而行](http://blog.kunx.org)

## 修复微信支付中安全问题及bug：

 * 修复sdk中的拼写错误
 * 修复php5.3之后默认禁用always_populate_raw_post_data(php7中直接去除了此特性)导致的xml获取失败的问题
 * 简单的自动加载机制
 * 账号信息放在配置文件中，以便修改
 * 更加简单的文件结构，只有两个文件夹，一个是core放置了类文件，cert文件夹放置证书
 * 完善的demo文件
> application/index/controller/Index.php


## 配置
请在配置文件添加配置信息，结构如下：
 <pre>
'wxpay'=>[
    'appid'=>'your appid',
    'mchid'=>'your mchid',
    'key'=>'your key',
    'appsecret'=>'your appsecret',
],
</pre>
## 日志放置在项目目录下的logs文件中，请确保文件夹可写




更多信息，请关注http://blog.kunx.org