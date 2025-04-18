# GraphicsPieces
In this repo, I've included short videos showcasing my tiny graphics objects, created using modern AI concepts. The projects were built on Three.js, with the framework provided, and I customized the fragment shaders to achieve unique effects.

## SDF - Cladding Pattern
When I studied architecture, facade/cladding was an important element to express the building's character. Inspired by this, I used Signed Distance Functions (SDF) to generate a customizable unit pattern for cladding.
Each piece consists of spheres and capped torus, with adjustable thickness and size for greater design flexibility. The capped torus function was adopted from [Inigo Quilez](https://www.shadertoy.com/view/tl23RK), and other maths are done by myself.

### No-Animation
<div align="center">
  <img src="https://github.com/user-attachments/assets/3ebc393a-c540-45c9-9b17-443a5220f9fe" width="700" />
</div>

### Size-Animation

<div align="center">
  <img src="https://github.com/user-attachments/assets/729fc169-648a-436f-b2ee-0d5679161e0d" width="700" />
</div>

The framerate was limited by my resources.

## SDF - Floating Ghosts

For this piece, I designed a stylized ghost character using neural SDFs; compensated for incomplete reconstruction of fine features (eyes/mouth) by applying Boolean subtraction to manually carve eye shapes in post-processing.
<div align="center">
  <img src="https://github.com/user-attachments/assets/a3cdeab3-1c81-419d-a9bf-7a31a677c5a8" width="700" />
</div>


## Volume Rendering
For this piece, I used Fractal Brownian Motion (FBM) with Perlin Noise to create an animation that forms a guided ghost shape from random noise. I referred to the cloud implementation on ShaderToy as inspiration.

I modified the shape composition and utilized Bezier curves to animate the components. Additionally, I applied exponential interpolation to control the strength of the FBM, transitioning from large to small values. To enhance the final frames, I incorporated linear color blending to add gradients to the ghost shape. The appearance of the eyes was a bit sudden, and I wish to explore a similar approach to create a more gradual "pop-up" effect in the future.

<div align="center">
  <img src="https://github.com/user-attachments/assets/1d666d0d-6dce-467b-b507-2a99d85248bc" width="700" />
</div>
<!--
![Ghost](https://github.com/user-attachments/assets/1d666d0d-6dce-467b-b507-2a99d85248bc)
-->

## 2D Gaussian Splatting

Optimized 2D gaussians with splat-size regularization to simulate pointillist rendering (inspired by Seurat); implemented 2D splatting in a fragment shader with explored controlled, artistic outputs.
<!--
<div align="center">
  <img src="https://github.com/user-attachments/assets/fe02df7e-0ac0-459e-ada5-2b0ecf58fbf9" width="700" />
</div>

-->

<div align="center">
  <img src="https://github.com/user-attachments/assets/4410d4f1-5100-47a3-9d0d-869cb8ac93e0" width="700" />
</div>

## Point-Based Dynamics


