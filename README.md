## getPerspectiveTransform

Javascript implementation of the getPerspectiveTransform() method from OpenCV
to calculate a perspective transformation matrix.

This affine transformation matrix is calculated from 8 points:
- the 4 first are the original points,
- the last 4 are the transformed points,

the result is a 4x4 matrix calculated for the transform of css parameter

```
<script src="./getPerspectiveTransform.js"></script>
<script>
  const op = [[-100, -49], [1, -91], [-12, 101], [117, 25]];
  const np = [[-160, -120], [160, -120], [-160, 120], [160, 120]]
  const m = getPerspectiveTransform(...op, ...np)
  document.querySelector('#image').style.transform = 'matrix3d(' + m.join(',') + ')';
</script>
```
![Perspective Transformation Result](demo.png)

See the [OpenCV documentation for this function](https://docs.opencv.org/4.5.5/da/d6e/tutorial_py_geometric_transformations.html)
(at the end of the page)

See [the demo](https://fccm.github.io/getPerspectiveTransform/demo.html)
