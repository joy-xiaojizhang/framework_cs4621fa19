# In-Class Exercise for Lecture 2 (2019-9-16)

## Vertex Shader Exercise: Involute of a Circle
In this exercise, you will draw the [involute of a circle](http://mathworld.wolfram.com/CircleInvolute.html), and add sliders for the radius (`a` in the formula) and the number of periods to go around the origin. The radius should be kept between 0 and 1. See the code of [Exhibit #1](exhibit01.html) for reference.

## Fragment Shader Exercise: Fractals! 
In this exercise, you will implement a slider that controls the rotation of the fractal around its center. The slider ranges from 1 to 360 degrees, and is initialized to 0 degrees. The rotation is counter-clockwise, and should work properly (i.e. always rotate around center of the fractal) upon modifying the values of `Center X`, `Center Y` and `Scale` using the sliders. Follow the steps below to complete the exercise:

* Modify the fragment shader
* Set up the corresponding GL Attribute
* Add the slider to the HTML view

Tips:
* Vector transformations follow this order: Scale, rotation, and transformation.

    ```transformed_vector = translation_matrix * rotation_matrix * scale_matrix * original_vector```
* [Wikipedia page](https://en.wikipedia.org/wiki/Rotation_matrix) on rotation matrix
* GLSL has `sin(x)` and `cos(x)` functions, as well as `radians(angle)` for converting degrees into radians.
