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
