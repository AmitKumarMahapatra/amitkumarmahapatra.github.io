## Master Theorem
- Master theorem is only applicable to the recursive equation which are in below format.

$$
T(n) = a * T(\dfrac{n}{b}) + f(n) \\
where \ a \geq 1 \ , \ b \gt 1 \\
and \\
f(n) is a +ve function
$$

- Master theorem is nothing but comparing 2 values.

$$
f(n) \ and \ n^{\log _{b} a}
$$

- There are 3 cases in Master Theorem
    - Case A

    $$
    if \ f(n) = O(n^{(\log_{b} a) \ - \ \epsilon}) \\
    where \ \epsilon > 0 \\
    then \ T(n) = \Theta(n^{(\log_{b}) a})
    $$

    - Case B

    $$
    if \ f(n) = \Omega(n^{(\log_{b} a) \ + \ \epsilon}) \\
    where \ \epsilon > 0 \\
    then \ T(n) = \Theta(f(n)) \\
    (and \ regularity \ condition)\\
    af(\dfrac{n}{b}) \leq c.f(n)
    $$ 

    - Case C
    
    $$
    if \ f(n) = \Theta(n^{(\log_{b} a)} \ . \ (log_{}n)^{k}) \\
    where \ k \geq 0 \\
    then \ T(n) = \Theta(n^{(\log_{b} a)} \ . \ (log_{}n)^{k + 1})
    $$

- This is what each case is really saying
    - Case A : $ n^{log_{b} a} $ is ***polynomial times bigger*** than $f(n)$. Not logarithmic. But higher than polynomial is fine.
    - Case B : $ n^{log_{b} a} $ is ***polynomial times smaller*** than $f(n)$. Not logarithmic time. Also is case B, the *regularity condition*, get passed in most cases. But you may need to check it if required.
    - Case C : $ n^{log_{b} a} $ and $f(n)$ both are equal or $ n^{log_{b} a} $ is logarithmic times smaller.

- Master Theorem always gives answer in $\theta$

### Example 1

$$
T(n) = 8 \ T(\dfrac{n}{2}) + n^2
$$

### Example 2

$$
T(n) = 2 \ T(\dfrac{n}{2}) + n^2
$$

### Example 3

$$
T(n) = T(\dfrac{n}{2}) + c
$$


### Example 4

$$
T(n) = 2 \ T(\dfrac{n}{2}) + n \ log_{} \ n
$$


### Example 5

$$
T(n) = 8 \ T(\dfrac{n}{2}) + n^4 log_{} \ n
$$


### Example 6

#### Case A

$$
T(n) = 2^n \ T(\dfrac{n}{2}) + n^2
$$

#### Case B

$$
T(n) = 2^n \ T(\dfrac{n}{2}) - n^2
$$

### Example 7

$$
T(n) = T(\sqrt{n}) + c
$$


### Example 8

$$
T(n) = T(\sqrt{n}) + log_{2}n
$$

### Example 8

$$
T(n) = 2^n \ T(\dfrac{n}{2}) + \dfrac{n}{log_{2}n}
$$

