# css3
##css3响应式布局
##弹性盒子模型实例

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>box model</title>
    <style>
        .box { 
            width: 100%; 
            height: 102px; 
            border:1px solid #ccc; 
            display: -webkit-box; 
            margin-top: 10px;
            /*-webkit-box-orient:vertical; */
            /*-webkit-box-direction:reverse; //布局方向normal:顺序  reverse：倒序*/
        }
        .box div { height: 100px; background:orange; color: #fff; font:30px/100px "STxihei"; text-align: center; border: 1px  solid #fff; }
        /*box-ordinal-group:设置元素的具体位置*/
        .box div:nth-of-type(1) { -webkit-box-ordinal-group:2; -webkit-box-flex:1; }
        .box div:nth-of-type(2) { -webkit-box-ordinal-group:4; -webkit-box-flex:1; }
        .box div:nth-of-type(3) { -webkit-box-ordinal-group:1; -webkit-box-flex:1; }
        .box div:nth-of-type(4) { -webkit-box-ordinal-group:5; -webkit-box-flex:1; }
        .box div:nth-of-type(5) { -webkit-box-ordinal-group:3; -webkit-box-flex:2; }
        .box li {
            width: 10%;
            height: 100%;
            border:1px solid #fff;
            background:#ccc;
        }
    </style>
</head>
<body>
    <div class="box">
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
        <div>5</div>
    </div>
    <div class="box">
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
        <li>5</li>
    </div>
</body>
</html>
```
