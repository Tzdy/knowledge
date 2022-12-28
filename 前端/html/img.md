图片设置错误的url时，为了能撑开图片，并且比例随父容器宽度变化（正方形）。
``` html
<div style="width: 100px;">
  <img src="error url" width="1" height="1" />
</div>
<script>
img {
  width: 100%;
  height: auto;
}
</script>
```
> 如果图片的比例不统一，还需要非错误情况下，img标签的比例固定，可以用padding-bottom+position: absolute;实现
