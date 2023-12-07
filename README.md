# 102architect

The main goal of this project was to develop a program to compute the coordinates of a point after several transformations using homogeneous coordinates.

### Installation

To use it dowload the executable and refeer to commands belows

## Usage

This project is directly a bash executable here is some usage : 

```
./102architect -h
```
```
USAGE
./102architect x y transfo1 arg11 [arg12] [transfo2 arg21 [arg22]] ...
DESCRIPTION
    x abscissa of the original point
    y ordinate of the original point
transfo arg1 [arg2]
    -t i j translation along vector (i, j)
    -z m n scaling by factors m (x-axis) and n (y-axis)
    -r d rotation centered in O by a d degree angle
    -s d reflection over the axis passing through O with an inclination angle of d degrees
```

## Examples

```
 ./102architect 5 0 -t -1 1
Translation along vector (-1, 1)
1.00 0.00 -1.00
0.00 1.00 1.00
0.00 0.00 1.00
(5.00, 0.00) => (4.00, 1.00)
```
```
./102architect 3 -1 -s 270
Reflection over an axis with an inclination angle of 270 degrees
-1.00 0.00 0.00
0.00 1.00 0.00
0.00 0.00 1.00
(3.00, -1.00) => (-3.00, -1.00)
```

## Authors

- [@ludeciel](https://www.github.com/ludecieldev)
