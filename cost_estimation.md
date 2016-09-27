# Cost Estimation

Using COCOMO Model.


## Basic COCOMO

Basic COCOMO computes software development effort (and cost) as a function of program size. Program size is expressed in estimated thousands of source lines of code (KLOC).


#### Software Project Class 

Our project is a Semi-detached project because we are a medium size team with mixed experience levels. 
The requirements are pretty rigid right now but we can extend our application later if we have time. 

According to Wikipedia, a project is Semi-detached if -> 

> Semi-detached projects - "medium" teams with mixed experience working with a mix of rigid and less than rigid requirements


#### Computations

```
Effort Applied (E) = 3.0 * (10) ** 1.12   # 39.54
Development Time (D) = 2.5 * E ** 0.38   # 9.055
People Required = E/D  # 4.367
```

#### Conclusion

According to the above computation using COCOMO model; 5 people are required to complete this project (coding period) in one month. 
Since we are taking out about 45 days for our development phase (design, coding, testing, deployment) and our team has a variety of skills, this seems like a fair estimate. 
