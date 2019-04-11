# Awesome MATLAB Operations

This repository aims at sharing interesting MATLAB operations I come across, and describing them in a smooth and simple manner.

<p align='center'>
  <img src='https://media.giphy.com/media/2Vp0UxNcA8TEQ/source.gif'>
  </p>

## [permute](https://www.mathworks.com/help/matlab/ref/permute.html)

This function permutates the dimensions of the array. Let's take some examples to make things more clear.

Say that we have the following array:

`>> A = [1 2; 3 4]`

``` 
A = 
1   2
3   4
``` 

If you run:

`>> permute(A,[1 2])`

You will get:

``` 
ans = 
1   2
3   4
``` 

Knowing that,

`1` ---> first dimension ---> row

`2` ---> second dimension ---> column

The above command is simply telling us to keep the first dimension as the rows dimension and the seond dimension as the column dimension. In other words, don't make any changes to your matrix.

If you however run the following command:

`>> permute(A,[2 1])`

This is telling us to set the first dimension (row) as the column dimension and the second dimension (column) as the row dimension. In other words, it is telling us to *flip* the dimensions, making the row a column and the column a row.

The output of the preceding command is thus:

``` 
ans = 
1   3
2   4
``` 

<p align='center'>
<img src="https://media.giphy.com/media/3o6gaYpCy25SPkchSE/source.gif">
</p>
