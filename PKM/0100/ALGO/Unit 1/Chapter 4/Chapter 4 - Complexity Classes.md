## Index
- [Complexity Classes](#section)
    - [Example 1](#example-1)
        - [Question](#question)
        - [Answer](#answer)
            - [Option 1](#option-1)
            - [Option B](#option-b)
                - [Applying Log](#applying-log)
                - [Fail Example 1](#fail-example-1)
                - [Fail Example 2](#fail-example-2)
                - [Substituting value](#substituting-value)
            - [Option C](#option-c)
            - [Option D](#option-d)
        - [Key Takeaway](#key-takeaway)
    - [Example 2](#example-2)
        - [Question](#question-1)
        - [Answer](#answer-1)
            - [Option A](#option-a-1)
            - [Option B](#option-b-1)
            - [Option C](#option-c-1)
            - [Option D](#option-d-1)
    - [Example 3](#example-3)
        - [Question](#question-2)
        - [Answer](#answer-2)
            - [Option A](#option-a-2)
            - [Option B](#option-b-2)
            - [Option C](#option-c-2)
            - [Option D](#option-d-2)
    - [Example 4](#example-4)
    - [Example 5](#example-5)
    - [Example 6](#example-6)
    - [Example 7](#example-7)
    - [Example 8](#example-8)
    - [Example 9](#example-9)
    - [Example 10](#example-10)
    - [Example 11](#example-11)
    - [Example 12](#example-12)
    - [Example 13](#example-13)
    - [Example 14](#example-14)
    - [Example 15](#example-15)
    - [Note for Stirling\'s Approximation](#note-for-stirlings-approximation)
    - [Properties of Asymptotic Notations](#properties-of-asymptotic-notations)
        - [Reflexive Property](#reflexive-property)
        - [Symmetric Property](#symmetric-property)
        - [Transitive Property](#transitive-property)
        - [Extra Property](#extra-property)

## Complexity Classes

1.  Decreasing Functions \[ $\frac{1}{n}$ , $\frac{1}{n^{2}}$ etc\]
2.  Constant Functions
    1.  $log(log(n))$
3.  Logarithmic Functions \[ $log\ n$, ${(log\ n)}^{2}$ etc \]
    1.  $$
4.  Polynomial Functions \[ $n^{c}\ where\ c \succ 0$ \]
    1.  Linear Functions
        1.  $nlog(n)$
        2.  $n$
    2.  Quadratic Functions
    3.  Cubic Functions
5.  Exponential Functions \[ $c^{n}\ where\ c \succ 1\ $ \]

## Example 1

### Question
Identify True and False Statements
1.  $1000\ nlog(n)\  = \  \odot (\frac{nlog(n)}{1000})$
2.  $\sqrt{log(n)}  = \  \odot (log(log(n)))$
3.  $if\ 0 < x < y\ then\ n^{x}\  = \odot (n^{y})$
4.  $n^{c}\  \neq \  \odot (c^{n})$

### Answer

#### Option 1
![Example 1 Option 1](./images/Example%201/Option%20A.jpg)

- This is the most basic example of the topic complexity class.
- The key take away from this option is that C will always help you if the difference is Constant.

#### Option 2
![Example 1 Option 2](./images/Example%201/Option%20B1.jpg)

- The above explanation is based on logical and mathematical fact, **Polynomial is always greater than logarithmic.**
- However, there are another 2 ways to solve a question like this
    1.  Apply Log
    2.  Substituting value
    
    ##### **Applying Log**
    ![](./images/Example%201/Option%20B2.jpg)
    - Applying log might fail in some cases as below. So be careful when using this method.

        ###### **Fail Example 1**

        $if\ x < y\ then\ c^{x} = \theta(c^{y}$)

        By solving this using Log Method

        $log(c^{x})\ \ \ \ \ \ \ \ log(c^{y})$

        $xlog(c)\ \ \ \ \ \ \ \ y\ log(c)$ $\ \ \ \ \ \ \ \ $ *(Canceling $log(c)$ both the sides)*

        $x\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ y$

        We know  $x < y$

        So we can take $x = n\ \&\&\ y = 2n$

        $n = \theta(2n)$

        So $c^{x} = \theta(c^{y})$

        But in reality $c^{x} = \odot (c^{y})$

        Because
        $2^{n} \neq \theta(2^{2n})\ \lbrack which\ is\ \theta(4^{n})\rbrack$

        ###### **Fail Example 2**

        $if\ x < y\ then\ n^{x} = \theta(n^{y})\ where\ x\ and\ y\ both\ are\ constants$

        By solving this using Log Method

        $log(n^{x})\ \ \ \ \ \ \ \ log(n^{y})$

        $xlog(n)\ \ \ \ \ \ \ \ log(n)$ $\ \ \ \ \ \ \ \ $ *(Canceling $log(n)$ both the sides)*

        $x\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ y$

        We know $x < y\ and\ both\ are\ constants\ so\ x = \theta(y)$

        Hence $n^{x} = \theta(n^{y})$

        But in reality $n^{x} = \odot (n^{y})$

        Because $n^{2} \neq \theta(n^{3})$

    ##### Substituting value
    ![](./images/Example%201/Option%20B3.jpg)
    - But taking values like this is not a good Idea though. Use this method only in the worst case scenario when you have no other option.
    - Still if you are using this method, then use very large values.
    - This method will fail for small values, because this is an Asymptotic comparison, not a pure mathematical one.

#### Option C
![](./images/Example%201/Option%20C.jpg)

#### Option D
![](./images/Example%201/Option%20D.jpg)

#### Key Takeaway
- $\omega$ means $\Omega$ But $\Omega$ does not necessarily means $\omega$
- $\circ$ means $\odot$ But $\odot$ does not necessarily means  $\circ$
- Subset and Superset Diagram
    - ![]()
- If $\theta$ is possible then  $\circ$ and $\omega$ not possible.
- If $\odot$ and $\Omega$ both are possible, then $\Theta possible.
- If $\Theta$ is not possible and the functions are comparable, one of $\omega$ or $\circ$ must be possible
- The way to compare the Asymptotic relation is in below order of priority
    -   Logical or strong Mathematical Proof
    -   Apply Log, But before applying, make sure, you are deleting the common terms
    -   Substitute will very big values, will give some idea
- If the difference is constant, the C will take care. But if the difference is a function, C can not help at all.

## Example 2

### Question

Identify True and False Statements
1.  $2^{n + 1} = \odot (2^{n})$
2.  $\frac{4^{n}}{2^{n}} = \odot (2^{n})$
3.  $2^{2n} = \odot (2^{n})$
4.  $64^{log(n)} = \odot (n^{10})$

### Answer

#### Option A
![]()

#### Option B
![]()

#### Option C
![]()

#### Option D
![]()

## Example 3

### Question

Identify True and False Statements
1.  $f(n) = \odot (({f(n))}^{2})$
2.  $f(n) = \odot (\frac{f(n)}{2})$
3.  $f(n) = \odot (f(\frac{n}{2}))$
4.  $if\ f(n) = \odot g(n)\ then\ 2^{f(n)} = \odot (2^{g(n)})$

### Answer

#### Option A
![]()

#### Option B
![]()

#### Option C
![]()

#### Option D
![]()

## Example 4

Identify True and False Statements
1.  $f_{1}(n) = 2^{n}$
2.  $f_{2}(n) = n^{log(n)}$
3.  $f_{3}(n) = n^{n}$
4.  $f_{4}(n) = n!$

## Example 5

Identify True and False Statements
1. $n > log(n)$
2. $n > {(logn)}^{2}$
3. $n > {(logn)}^{10}$
4. $n > {(logn)}^{100000}$

## Example 6

Identify the Asymptotic Relation.

$\log_{2}(n)\ ?\ \log_{3}(n)$

## Example 7

Identify the Asymptotic Relation.

$2^{n}\ ?\ 3^{n}$

## Example 8

Identify True and False Statements
1.  $100000\  = \  \odot (1)$
2.  $\frac{1}{n} = \theta(1)$
3.  $1000\  = \ \theta(1)$
4.  $1000\  = \  \odot (\frac{1}{n})$

## Example 9

$let\ f(n),\ g(n)\ and\ h(n)\ be\ 3\  + ve\ functions,\ defined\ as\ below$

1.  $f(n) = \odot (g(n))\ \&\&\ g(n) \neq \odot (f(n))$
2.  $g(n) = \odot (h(n))\ \&\&\ h(n) = \odot (g(n))$

Then Identify True and False Statements
1.  $f(n).g(n)\  = \odot (g(n).h(n))$
2.  $f(n) + g(n)\  = \odot (h(n))$
3.  $h(n)\  = \theta(f(n))$
4.  $g(n).h(n)\  = \theta(h(n).h(n))$

## Example 10

$$
\begin{equation}
\ f(n)=
    \begin{cases}
        2^n & \text{if n\ is\ even} \\
        n & \text{if n\ is\ odd} \\
    \end{cases}
\end{equation}
$$

$$
\begin{equation}
\ g(n)=
    \begin{cases}
        2^n & \text{if n\ is\ odd} \\
        n & \text{if n\ is\ even} \\
    \end{cases}
\end{equation}
$$

Identify the Asymptotic relation between $f(n)\ and\ g(n)$

## Example 11

$$
\begin{equation}
\ f(n)=
    \begin{cases}
        n^3 & \text{if\ 0 <> n < 100} \\
        n^5 & \text{if \ n $\geq$ 100} \\
    \end{cases}
\end{equation}
$$

$$
\begin{equation}
\ g(n)=
    \begin{cases}
        n^7 & \text{if\ 0 < n < 10000} \\
        n^2 & \text{if \ n $\geq$ 10000} \\
    \end{cases}
\end{equation}
$$

Identify the Asymptotic relation between $f(n)\ and\ g(n)$

## Example 12

$f(n) = \ n^{1 + sin(n)\ }$

$g(n) = \ n^{1 + cos(n)\ }$

Identify the Asymptotic relation between $f(n)\ and\ g(n)$

## Example 13

$f(n) = \ n^{1 + sin(n)\ }$

$g(n) = \ n^{2 + cos(n)\ }$

Identify the Asymptotic relation between $f(n)\ and\ g(n)$

## Example 14

$f(n) = \ n^{1 - cos(n)\ }$

$g(n) = \ n^{2 + sin(n)\ }$

Identify the Asymptotic relation between $f(n)\ and\ g(n)$

## Example 15

$$
f_{1} = n^{log(n)} \\
f_{2} = {(log(n))}^{log(n)} \\
f_{3} = n! \\
f_{4} = (log(n))! \\
f_{5} = log(n!) \\
f_{6} = \\
f_{7} = (log(log(n)))! \\
f_{8} = 2^{n} \\
f_{9} = n^{} \\
$$

Arrange in Asymptotic Increasing order.

## Note for Stirling\'s Approximation

$n!\  < \ n^{n}$ Strictly

SO $\ n! = \odot (n^{n})$

But $log(n!) = \theta(nlogn)$ According to Stirling\'s Approximation.

Proof:

$n!\  \equiv \ \ \left( \frac{n}{e} \right)^{n}$

$\Rightarrow \ log(n!) \equiv log() + nlog(\frac{n}{e})$

$\Rightarrow \ log(n!) \equiv \frac{1}{2}log(2\pi e) + \frac{1}{2}log(n) + nlog(n) - nlog(e)$

$\Rightarrow \ log(n!) \equiv \ K\  + \ log(n)\  + \ nlog(n)\  + \ nK_{1}$

$\Rightarrow \ log(n!) \equiv \ \theta(nlog(n))$

# Properties of Asymptotic Notations

## Reflexive Property

$f(n) = \odot (f(n))$

$f(n) = \Omega(f(n))$

$f(n) = \Theta(f(n))$

$\odot$ $\Omega$ and $\Theta$ satisfy this property.

$\circ$ and $\omega$ however, does not satisfy this property.

## Symmetric Property

$f(n) = \odot (g(n))$ then $g(n) = \odot (f(n))$

What will pass ?

What will not pass ?

## Transitive Property

$f(n) = \odot (g(n))$ and $g(n) = \odot (h(n))$

$then\ f(n) = \odot (h(n))$

$\odot$, $\Omega$, $\Theta$, $\circ$ and $\omega$ all will satisfy this
condition.

## Extra Property

$f(n) = \odot (g(n))$ and $d(n) = \odot (e(n))$

$then$

$f(n)\  + \ d(n) = \odot (g(n) + e(n))\ or\ MAX(g(n),\ e(n))$

$f(n).g(n) = \odot (g(n).e(n))$
