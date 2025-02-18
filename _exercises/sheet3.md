---
layout: default
mathjax: true
title:  Sheet 3
date:   2022-11-03 09:33:19 +0100
categories: exercises 
---

## Sheet 3

<!--
In this class you will receive help on the implementation of the
sparse vectors and sparse matrices for `asg1`. 

You will also work on the following tasks about data visualization.
-->


Exercises with a star on the side must be done
before coming to the class.  Exercises with a hat on the side will be
tackled in class.



### Task 1* -- Matplotlib: Plotting in Python

Write a function to plot the curve $f(x) = \frac{1}{x-1}$ on the domain $[-2,6]$.

1. Although $f(x)$ has a discontinuity at $x=1$, a single call to `plt.plot()` in the usual way will make the curve look continuous.
Split up the domain into $[-2,1)$ and $(1,6]$.
Plot the two sides of the curve separately so that the graph looks discontinuous at $x=1$.

2. Plot both curves with a dashed magenta line.
Set the keyword argument `linewidth` (or `lw`) of `plt.plot()` to $4$ to make the line a little thicker than the default setting.

3. Use `plt.xlim()` and `plt.ylim()` to change the range of the $x$-axis to $[-2,6]$ and the range of the $y$-axis to $[-6, 6]$.


### Task 2^


Write a function that plots the functions $\sin(x)$, $\sin(2x)$,
$2\sin(x)$, and $2\sin(2x)$ on the domain $[0, 2\pi]$, each in a
separate subplot of a single figure.

1. Arrange the plots in a $2\times 2$ grid of subplots.
   
2. Set the limits of each subplot to $[0, 2\pi]\times[-2,2]$.
    (Hint: Consider using `plt.axis([xmin, xmax, ymin, ymax])` instead
    of `plt.xlim()` and `plt.ylim()` to set all boundaries
    simultaneously.)
	
3. Use `plt.title()` or `ax.set_title()` to give each subplot an appropriate title.

4. Use `plt.suptitle()` or `fig.suptitle()` to give the overall figure a title.

5. Use the following colors and line styles.
   - $\sin(x)${: green solid line.} 
   - $\sin(2x)${: red dashed line.}
   - $2\sin(x)${: blue dashed line.} 
   - $2\sin(2x)${: magenta dotted line.}



### Task 3^

Using the results from `benchmark.py` of assignment 1, compare the
growth curve of your implementation and Numpy implementation of matrix
multiplication. Consider only square matrices of varying size. Try to
perform logarithmic transformations on the axis. Which transformation
leads to a linear growth? What do the plots say about the growth
function (ie, polynomial or exponential) of the procedures?  [You will
need to modify `benchmark.py` to print out the results for different
sizes of the matrices. You should put the results in a file. Then your
script for plotting should read the data from the file and plot the
growth curves.]


