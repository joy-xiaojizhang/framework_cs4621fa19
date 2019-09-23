# Exercise: Alpha Blending of Two Textures
In this exercise, you will modify a program that displays one image to display two images using multi-texturing. Specifically, you will add a texture for the [Patrick Star image](img/patrick-star.png), and apply Alpha Blending to blend it over the existing Spongebob image. You will also control the Alpha value with a slider, ranging from 0 to 1 and initialized to 0. Follow the steps below to complete the exercise:

* Create a second texture for Patrick Star and load the image
* Set up binding for the second texture
* Add Alpha Blending logic to the fragment shader
* Add the slider for alpha

Tips:
* Alpha Blending formula:

    ```out_color = alpha * new_img_color + (1.0 - alpha) * old_img_color```

* Use callback for loading images. We want to execute `runWebGL` upon successfully loading both images.

* The WebGL Fundamentals site has a useful [example](https://webglfundamentals.org/webgl/lessons/webgl-2-textures.html) on playing with multiple textures.
