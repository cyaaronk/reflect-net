# Reflect-Net
Reflection generation using convolution neural networks

## Overview
Reflection generation is a difficult task in the Machine learning field because input image features are often not aligned with ground truth image features. For example, a mirror image (in a plane mirror) is a reflected duplication of an object that appears almost identical, but is reversed in the direction perpendicular to the mirror surface. As such, we need to develop a new neural network that is capable of moving image features to a different location.

The contribution of this project is three fold. First, to the best of our knowledge, our work is the first attempt to generate reflections using machine learning algorithms. Second, we present the first 2D-convolutional based network that is capable of moving image features to different locations where no auto-regression model is used in the process. Third, we provide the world's first publicly available dataset that can be used for research in the related area.

## Related work
Reflection generation was traditionally accomplished by Screen Space Reflection(SSR). It uses a technique known as ray marching to determine the reflected point and potential candidates of reflected objects in a scene. This is done by reversely tracing the light ray coming out from the camera, onto the reflected point, and onto the reflected geometry by probing a set of scene's position and depth in each iteration. It then reuses the color that is already rendered in screen space as an approximation of the final reflected color, thus the name Screen Space Reflection because it is doing reflection of itself onto itself. However, this method has the limitation of not generating reflections that are accurate enough when the reflected object has a complex shape and color.

Pure ray tracing, on the other hand, does not reuse the color on the screen but calculate the color of reflected light by tracing every light ray produced by every single source of lighting in the scene. So instead of stopping at the reflected object, the reverse ray tracing continues to trace its path back to the light sources like a lamp or the sun, and calculate the reflected color based on reflected objects' diffuse color, the color of light source and more. This method is computationally expensive and is not suitable for quick rendering.

## Our method
(Pending for update)

## Results
<img src=results/inp1.png width=200 height=200> <img src=results/gt1.png width=200 height=200> <img src=results/pred1.png width=200 height=200>

<img src=results/inp2.png width=200 height=200> <img src=results/gt2.png width=200 height=200> <img src=results/pred2.png width=200 height=200>

<img src=results/inp3.png width=200 height=200> <img src=results/gt3.png width=200 height=200> <img src=results/pred3.png width=200 height=200>

<img src=results/inp4.png width=200 height=200> <img src=results/gt4.png width=200 height=200> <img src=results/pred4.png width=200 height=200>

## Dataset
(Pending for update)
