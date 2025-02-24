## Mathematical Representation

Image translation can be expressed as a function that maps pixel coordinates from one location to another. Given an image function \( I(x, y) \), a translation by \( (t_x, t_y) \) can be defined as:

\[
I'(x, y) = I(x - t_x, y - t_y)
\]

where:

- \( I(x, y) \) is the original image,
- \( I'(x, y) \) is the translated image,
- \( t_x \) and \( t_y \) are the translation distances along the x-axis and y-axis, respectively.

### Homogeneous Coordinates Representation

In matrix notation, translation can be expressed using homogeneous coordinates. The transformation matrix for 2D translation is:

\[
T = \begin{bmatrix} 1 & 0 & t_x \\ 0 & 1 & t_y \\ 0 & 0 & 1 \end{bmatrix}
\]

A point \( (x, y) \) in homogeneous coordinates is represented as \( P = [x, y, 1]^T \), and the translated point \( P' \) is obtained by:

\[
P' = T P = \begin{bmatrix} 1 & 0 & t_x \\ 0 & 1 & t_y \\ 0 & 0 & 1 \end{bmatrix} \begin{bmatrix} x \\ y \\ 1 \end{bmatrix} = \begin{bmatrix} x + t_x \\ y + t_y \\ 1 \end{bmatrix}
\]

### Example Calculation

Suppose we have an image with a pixel at \( (5, 3) \), and we want to translate it by \( (t_x, t_y) = (2, -4) \). The new coordinates will be:

\[
\begin{bmatrix} 5 + 2 \\ 3 - 4 \end{bmatrix} = \begin{bmatrix} 7 \\ -1 \end{bmatrix}
\]

This means the pixel previously at \( (5, 3) \) now appears at \( (7, -1) \) in the translated image.
