## Recursive Tree Method
- It is applied in below type of recursive functions

$$
T(n) = T(\dfrac{n}{3}) + T(\dfrac{n}{2}) + n
$$

### Example 1

$$
T(n) = T(\dfrac{n}{3}) + T(\dfrac{2n}{3}) + n
$$

![](./images/Example%201.jpg)

### Example 2

$$
T(n) = T(\dfrac{n}{5}) + T(\dfrac{2n}{5}) + n
$$

![](./images/Example%202.jpg)

### Example 3

$$
T(n) = T(\dfrac{n}{2}) + T(\dfrac{n}{3}) + c
$$

![](./images/Example%203.jpg)

### Example 4

$$
T(n) = T(n-1) + T(\dfrac{n}{2}) + T(\dfrac{n}{3}) + c
$$

![](./images/Example%204.jpg)

### Example 5

$$
T(n) = T(\dfrac{n}{3}) + T(\dfrac{2n}{2}) + n^2
$$

![](./images/Example%205.jpg)


### Notes
- Just a claver trick here, even if the recursive equation is written as 2 different factors, we can solve slightly further and then apply Master's theorem or Substitution method. No need to go for Recursion Tree Method

$$
T(n) = T(\dfrac{n}{2}) + T(\dfrac{n}{2}) + n
\\
=> T(n) = 2T(\dfrac{n}{2}) + n
$$

- So directly or indirectly, if there is 1 function call, then we can go with Substitution method or Master's theorem (depending upon the format), and if there are 2 different recursive call (like above examples), we should go with Recursive tree method.