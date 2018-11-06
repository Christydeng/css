# css
Note about css

1.元素居中常用方法
① flex布局

html

<div class="ourter">
    <div class="inner"></div>
</div>

css
.ourter {
  width: 200px;
  height: 200px;
  background-color: pink;
  display: flex;
  justify-content: center;
  align-items: center;
}

.inner {
  width: 100px;
  height: 100px;
  background-color: yellow;
}

②
css
div {
    width: 100px;
    height: 100px;
    position: absolute;
    left: 50%;
    top: 50%;
    margin-left: -50px;
    margin-top: -50px;
}

margin-left, margin-top设置技巧： 分别为宽和高的一半

2. Scss混合宏的使用

    @mixin mt($value) {
        margin-top: $value;
        }
        
    .header {
        display: inline-block;
        @include mt(20px);
        nav {
            color: pink;
            @include mt(10px);
        }
        p {
            color: blue;
            @include mt(5px);
        }
    }
    
    Scss继承的使用
    .mt {
        margin-top: 10px;
    }
    
    header {
        color: red;
        @extend .mt;
        span {
            color: red;
            @extend .mt;
         }
    }
    
    Scss占位符的使用
    
    %mt {
        margin-top: 10px;
    }
    
    header {
        color: red;
        @extend %mt
        span {
            background: yellow;
            @extend %mt;
        }
    }
    
3. 用css画三角形

<div class="divBox"></div>

.divBox {
  width: 0px;
  height: 0px;
  border-width: 30px;
  border-style: solid;
  border-color: transparent transparent yellow;
}
    
 
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
