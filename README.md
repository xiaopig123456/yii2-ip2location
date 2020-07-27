# Yii2 Ip to Location

## 安装

安装这个扩展的首选方式是通过 [composer](http://getcomposer.org/download/).

执行

```bash
composer require --prefer-dist xiaopig123456/yii2-ip2location
```

## 根据IP查询
```php
use \wsl\ip2location\Ip2Location;
// 查询ip
$ipAddress = Ip2Location::getIpAddress();
echo $ipAddress;
// 8.8.8.8

// 根据查询地址
$locationModel = Ip2Location::getIpAddress($ipAddress);
print_r($locationModel->toArray());
// Array
// (
//     [country] => 美国
//     [province] => null
//     [city] => null
//     [description] => 加利福尼亚州圣克拉拉县山景市谷歌公司DNS服务器
// )
```
## 数据库最新版本
数据库最后更新版本2020年7月25日