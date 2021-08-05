## a标签的用法

a标签用以：

1.跳转外部页面
2.跳转内部锚点
3.跳转到邮箱或者电话等

a标签的属性有:

1.href添加地址
2.target跳转方式
3.download下载
4.rel=noopener防止window.opener被滥用，在使用target时加上


a标签的格式：
`<a href="" target="" rel="noopener norefferrer"></a>`

## img标签的用法

* 发送get请求，然后展示一张图片

* 一定要有src

img标签的属性有：

1.src图片地址
2.alt加载失败时的解释
3.height图片高度
4.width图片宽度
5.onload加载成功提示
6.error加载失败提示，在之后添加新的图片地址，可以重新加载备用图片

img标签的格式：

```
<img src="" alt="" height=""/>
<script>
        xxx.onload = function() {
            console.log('图片加载成功 ')
        }

        xxx.error = function() {
            console.log('图片加载失败 ');
            xxx.scr = "";
        }
    </script>
 ```
 
## table标签的用法

表格标签，里面含有:

```
<thead>

<tbody>

<tfoot>

<tr>

<th>

<td>
```
table 标签的使用方法：
 
```
<table>
<thead><tr><th></th><td></td></tr></thead>
<tbody><tr><th></th><td></td></tr></tbody>
<tfoot><tr><th></th><td></td></tr></tfoot>
</table>
```

注意<tbody>不可以少
 
  
## 其他感想
 
form标签:发送get或者post请求，然后刷新页面
  
form标签一定有一个type="submit"按钮
  
form标签的属性：
  
1.action
2.method
3.target
4.autocomplete
  
  
注意button和input的区别，前者可以添加任何标签，后者不行
将img标签的宽度设置为100%，可以适应屏幕自动调整大小
