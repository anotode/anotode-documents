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

The formula to calculate people required COCOMO model goes as -- 

```
Effort Applied (E) = 3.0 * (KLOC) ** 1.12 [ man-months ]
Development Time (D) = 2.5 * (Effort Applied) ** 0.38 [months]
People required (P) = Effort Applied / Development Time [count]
```

Now the first step is to calculate KLOC. Here is what we came up with after some analysis. 

<table>
<tr>
	<th>Sub-project</th>
	<th>KLOC</th>
</tr>
<tr>
	<td>Android App</td>
	<td>3</td>
</tr>
<tr>
	<td>Backend Server</td>
	<td>2.5</td>
</tr>
<tr>
	<td>Browser Extensions</td>
	<td>3</td>
</tr>
<tr>
	<td>Frontend / website</td>
	<td>1.5</td>
</tr>
</table>

Total KLOC = 10

```python
E = 3.0 * (10) ** 1.12   # 39.54
D = 2.5 * E ** 0.38   # 9.055
P = E/D  # 4.367
```

#### Conclusion

According to the above computation using COCOMO model; 5 people are required to complete this project (coding period) in one month. 
Since we are taking out about 45 days for our development phase (design, coding, testing, deployment) and our team has a variety of skills, this seems like a fair estimate. 
