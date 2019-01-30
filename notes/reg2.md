## 1. 匹配url的正则

```javascript
var reg = /https?|ftp|file:\/\/[-A-Za-z0-9+@/&%#=～_|:;.,!]+[+@/%#=+_~|]/
```

## 2. 匹配邮箱的正则

登录名@主机名.域名。登陆名，2-16位，以字母开头，以字母和数字结尾。顶级域名一般为2-4位， 如com/cn

```javascript
var reg = /[A-Za-z\d]+[_]*[A-Za-z\d]+@[A-Za-z\d]+\.[A-Za-z]{2,4}/
```

## 3. 匹配IP的正则

```javascript
var reg = /((2[0-4]\d|25[0-5]|[01]?\d\d?)\.){3}(2[0-4]\d|25[0-5]|[01]?\d\d?)/
```

## 4. 匹配文件路径的正则

e.g. /Users/wangsiyuan/Desktop/image.svg

```javascript
var reg = /(\/[\w]+)+\.[A-Za-z]+/
```

## 5. 匹配合法数字的正则

```javascript
var reg = /[-+]?\d?\.?\d+/
```

## 6. 匹配手机号的正则

```javascript
var reg = /1(3|4|5|7|8)\d{9}/
```

## 7. 判断html标签的正则

```javascript
var reg = /(?<=<\w+>).*(?=<\/\1>)/
```

## 8. 去除首尾空白字符
```javascipt
function trim(str){
    return str.replace(/^\s+|\s+$/g, '')
}
```
