图片设置错误的url时，为了能撑开图片，并且比例随父容器宽度变化。
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
