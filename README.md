# Double-Cone

A **double cone** is a geometric shape formed by two identical cones that share a common vertex and are oriented in opposite directions along the same axis. It looks like two cones placed tip-to-tip. Double cones are often used in mathematics and physics to describe certain types of surfaces or trajectories.

### Explanation of the Equation

The parametric equations you provided define the surface of the double cone in 3D space. Let's break down the equations:

1. **Parametric Equations**:
   ![Image](https://github.com/user-attachments/assets/b4a22660-18e4-4960-bd91-dd1ba4ac28bf)

   Here, \( u \) and \( v \) are parameters that vary over specific ranges:
   - \( 0 \leq u \leq 2\pi \) (angle around the axis)
   - \( -2 \leq v \leq 2 \) (height along the axis)

2. **Variables**:
   - \( u \): This parameter controls the angle around the axis of the double cone. It ranges from \( 0 \) to \( 2\pi \), which means it sweeps a full circle around the axis.
   - \( v \): This parameter controls the height along the axis of the double cone. It ranges from \(-2\) to \(2\), which means it covers the length of the double cone.

3. **Components**:
   - **\( x = v \cos(u) \)**: This equation defines the x-coordinate of a point on the surface. The \( v \) term scales the radius of the cone, and \( \cos(u) \) determines the position around the circle at that height.
   - **\( y = (e^{\sin(v)} - 1) \cos\left(u + \frac{\pi}{3}\right) \)**: This equation defines the y-coordinate. The term \( e^{\sin(v)} - 1 \) introduces a sinusoidal variation in the radius, and \( \cos\left(u + \frac{\pi}{3}\right) \) shifts the angle by \( \frac{\pi}{3} \).
   - **\( z = 1 - e^{c \cos(v)} \cos\left(u - \frac{2\pi}{3}\right) \)**: This equation defines the z-coordinate. The term \( e^{c \cos(v)} \) introduces another exponential variation, and \( \cos\left(u - \frac{2\pi}{3}\right) \) shifts the angle by \( \frac{2\pi}{3} \).

### Visualization in Code

In the provided JavaScript code using Three.js, the double cone is created by generating points in 3D space based on these parametric equations. Here's a breakdown of the code:

1. **Points Generation**:
   - The nested loops iterate over the parameters \( u \) and \( v \) to generate points on the surface of the double cone.
   - For each combination of \( u \) and \( v \), the coordinates \( (x, y, z) \) are calculated using the parametric equations.

2. **Geometry and Material**:
   - The points are stored in a `THREE.BufferGeometry` object, which is used to define the shape.
   - A `THREE.PointsMaterial` is used to render the points with a specific color and size.

3. **Animation**:
   - The double cone is animated by rotating it around the x and y axes in the animation loop.

This setup allows you to visualize the double cone in a 3D space and animate it to see its structure from different angles. The equations define the unique shape of the double cone, and the code translates these equations into a visual representation.
