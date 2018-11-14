## 问题描述：
a标签添加:hover，在ios上需要点击2次才能跳转

#### 解决方案： 
使用js跳转代替a标签的跳转事件

```
     $('a').on('click touchend', function(e) {
        var el = $(this);
        var link = el.attr('href');
        window.location = link;
    });
```



## 问题描述 
a标签或者onclick事件在移动端会出现高亮效果

#### 解决方案
将对应元素添css属性： -webkit-tap-highlight-color:rgba(0,0,0,0);

