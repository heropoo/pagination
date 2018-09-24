# pagination
Pagination

## 使用方法

install via composer
```
composer require heropoo/pagination
```

```php
$user_total = 100;
$page_size = 10;
$page = new Page($user_total, $page_size);
//获取分页 offset 参数
$limit = $page->getLimit();   //等于 $page_size
$offset = $page->getOffset();
//输出的html
$html = $page->getHtml();
echo $html;
```
