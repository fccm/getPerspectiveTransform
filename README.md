# getPerspectiveTransform
使用js实现opencv中的getPerspectiveTransform方法，计算透视变换矩阵，参数是8个点，前四个是原始点，后四个是变换后的点，

```
<script src="./getPerspectiveTransform.js"></script>
var m = getPerspectiveTransform([-150, -150], [150, -150], [-150, 150], [150, 150], [-150, -150, 0, 1], [323, -207, 0, 1], [-150, 150, 0, 1], [150, 150, 0, 1]);
 console.log(m);
```
