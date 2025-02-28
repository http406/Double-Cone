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
   ![Image](https://github.com/user-attachments/assets/fbcd15be-4999-4887-9fa4-d49c76340785)
   
4. **Components**:
   ![Image](https://github.com/user-attachments/assets/19072435-7f3d-424f-88b3-819c322fee6b)

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
