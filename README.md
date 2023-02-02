# Reconstructing an image from a corrupt image and an incomplete image

Given the flattened matrix of the representation of an incomplete image, the transformation applied on the sparse representation of the image to generate the actual image and the incomplete image, solve the problem of least squares (minimize the 2 norm) to obtain the sparse vector and the actual image.

Say x = As
where x - flattened matrix of the actual image
s - sparse representation of the image x
A - transformation

then minimize $||y - Cs||^2$ where we know that y is the incomplete image obtained by applying a transformation C on the sparse representation s.

The solution to the least squares problem is given by 
s = $(C^T*C)^(-1)*C^T*y$
