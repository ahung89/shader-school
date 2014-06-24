# Reflections

In this exercise, you will figure out how to represent a reflection as a matrix transformation.  Reflections flip a vector along a given axis.  Specifically, the reflection of a point p along the axis n is defined to be:

```glsl
vec3 reflectPoint(vec3 p, vec3 n) {
  return p - 2.0 * dot(n, p) * n / dot(n, n);
}
```

## Exercises

The above function is again linear in `p` so it can be translated into a matrix.  Do this now by modifying the file `reflect.glsl` and writing a GLSL function to compute this quantity.