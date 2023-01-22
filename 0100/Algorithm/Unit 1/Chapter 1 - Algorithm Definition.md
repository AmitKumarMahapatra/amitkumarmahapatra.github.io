## Algorithm Definition

It is a combination of a **sequence** of **finite steps** to **solve a
problem**.

- **Sequence** : You cannot swap 2 logical steps.
- **Finite Steps** : Every algorithm should be finite and every step must be
mandatory or else it is not required in the algorithm itself.
- **Solve a problem** : The algorithm must be solving a problem.

## Properties of Algorithm

### Property 1

It should terminate after a finite time.
```c
  while(1) {
    print ("Infinity");
  }
```
The above code will not terminate in finite time. So it is not an
algorithm.

### Property 2

It should produce one output directly or indirectly.

### Property 3

Every statement in algorithm must be effective

```c
  x = x
```

The above assignment is useless. So this kind of statement should not be
present in any algorithm.

### Property 4

Every algorithm must be deterministic.

### Property 5

Algorithms must be independent of programming language.

### Why Properties of Algorithm is Important?

I have written a code. Now I want to know if it's an algorithm or not.
To know that, we need to know the properties of algorithms.

## Steps required to design an algorithm

### Step 1

Know Problem Definition.

*Mostly MBAs and Client do this discussion. Client and
Developer never talk*

### Step 2

Select the Design Technique.

In the Algorithm subject we have lots of algorithms.
For example,

-   Divide and Conquer
-   Greedy Technique
-   Dynamic Programming Technique
-   Branch and Bound Technique
-   Backtracking Technique, etc

The expert will try to map the problem to the most suitable algorithm.
Only experts can do this properly. Because he knows which algorithm
techniques can be applied to solve the problem. Among all of those
candidate algorithms, which one is the best performing.

It\'s like an expert web developer already has lots of templates. When a
client comes to him, he will show him various sample templates. But a
fresher one will always do things from scratch. That\'s the difference
between an expert and a fresher.

### Step 3

Draw Flow chart

### Step 4

Verification

### Step 5

Coding

### Step 6

Analysis (Time and Space Complexity Analysis)

## Note

Only CSE People can do the 2nd and 6th step, No one else can.