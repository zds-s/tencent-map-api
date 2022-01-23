# 腾讯地图webservices的php封装
## 安装

---
```shell
composer require death_satan/tencent-map-api -vvv
```
---

## 使用

---
```php
$key = '';//腾讯地图key
$app = new \DeathSatan\TencentMapApi\Application($key);

//地址转经纬度
$data=$app->api()->addressResolution('北京市');
var_dump($data);
/**
* echo 
 * 
    ["adcode"]=>
    string(6) "110114"
  }
  ["address_components"]=>
  array(5) {
    ["province"]=>
    string(9) "北京市"
    ["city"]=>
    string(9) "北京市"
    ["district"]=>
    string(9) "昌平区"
    ["street"]=>
    string(0) ""
    ["street_number"]=>
    string(0) ""
  }
  ["similarity"]=>
  float(0.8)
  ["deviation"]=>
  int(1000)
  ["reliability"]=>
  int(1)
  ["level"]=>
  int(2)
}
 */
```
---