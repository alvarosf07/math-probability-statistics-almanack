You are given N variables $x_{1,t},...,x_{N,t}$  which we observe at different discrete points in time t. 
Our goal is to explain a variable yt using linear regression, that is,
<br/>

$y=a+&sum;I_k&beta;_k x_{k,t}+&epsilon;_t$

<br/>
where &epsilon; is an error term, $I$ is an indicator variable that equals 1 if the variable $x_k$ is included in the
model, zero otherwise, $&beta;_k$ are the regression coefficients, $a$ is a constant. Assume properties are such that
ordinary least squares can be applied to estimate the coefficients $k$.

As an example, assume we have N=4 and choose $I_1 = I_4 = 1$ and $I_2 = I_3 = 0$, the resulting model is
$y_t = a + &beta;_1 x_{1,t} + &beta;_4 x_{4,t} + &epsilon; $. In the following, we consider the general case with N variables.

- How many different models (i.e., combinations of variables) can you construct using the N variables $x_1, ..., x_N$?
- How would you perform model selection? That is, which regression model would you select as the
  "best" model among the linear models in this family? You do not have to implement this part.
- Assume that a member of our team developed a statistical test that you can apply to your models.
The test creates a test statistic for each model and the true distribution of the test statistics is known.
The null hypothesis is that the model is "not good", the alternative is that the model is "good". You
apply the test to all of the K models that you constructed and choose the confidence interval 1 - &alpha; equal to 95%.
  + If $K$ is very large, how many models do you expect to be considered "good" by the test?
  + Assume that 100% of the models that you test are "not good". How many models will be considered "good" in this case?

