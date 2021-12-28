# 入群欢迎语素材管理

> 微信文档：https://work.weixin.qq.com/api/doc/90000/90135/92366

## 添加入群欢迎语素材

企业可通过此API向企业的入群欢迎语素材库中添加素材。每个企业的入群欢迎语素材库中，最多容纳100个素材。

```php
$template = $app->group_welcome_template;

$template->add([
    'text' => [
        'content' => '亲爱的%NICKNAME%用户，你好'
    ],
    'video' => [
        'media_id' => '3slzN7WlXH1Ngy3Z4hq0AQZKqKd3l9F23Tjac1i4qqWidD1QCaJTW7sEBhQQVNLe5'
    ]
]);
```

## 编辑入群欢迎语素材

企业可通过此API编辑入群欢迎语素材库中的素材，且仅能够编辑调用方自己创建的入群欢迎语素材。

```php
$template = $app->group_welcome_template;

// 根据模版ID进行编辑
$template->edit('msg2MgBEgAATurBYDPgS32DfSt5vdzaHA', [
    'text' => [
        'content' => '亲爱的%NICKNAME%用户，你好呀'
    ],
    'video' => [
        'media_id' => '3slzN7WlXH1Ngy3Z4hq0AQZKqKd3l9F23Tjac1i4qqWidD1QCaJTW7sEBhQQVNLe5'
    ]
]);
```

## 获取入群欢迎语素材

企业可通过此API获取入群欢迎语素材。

```php
$template = $app->group_welcome_template;

$template->get('msg2MgBEgAATurBYDPgS32DfSt5vdzaHA');
```

## 删除入群欢迎语素材

企业可通过此API删除入群欢迎语素材，且仅能删除调用方自己创建的入群欢迎语素材。

```php
$template = $app->group_welcome_template;

$template->del('msg2MgBEgAATurBYDPgS32DfSt5vdzaHA');
```




