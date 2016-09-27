# Cost Estimation

Using COCOMO Model.


## Basic COCOMO

Basic COCOMO compute software development effort (and cost) as a function of program size. 
Program size is expressed in estimated thousands of source lines of code.


#### Software Project Class 

> Semi-detached projects - "medium" teams with mixed experience working with a mix of rigid and less than rigid requirements

#### Computations

```
Effort Applied (E) = 3.0 * (10) ** 1.12   # 39.54
Development Time (D) = 2.5 * E ** 0.38   # 9.055
People Required = E/D  # 4.367
```

#### Conclusion

5 people are required to complete this project (coding period) in one month. 

