# css
Note about css

1.元素居中常用方法

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
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
