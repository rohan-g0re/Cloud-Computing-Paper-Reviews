

# Introduction

### Problems Tackled and How is it better than competitors

```

- Current frameworks provide methods for management of computing resources, but they lack the methods to provide control over memory resources.

- Also, there are a few existing frameworks like Pregel and HaLoop which in-memory data handling but they only support a few types of patterns, such as graph computations && map-reduce looping. So they are not really generic

- Defining a programming interface that provide fault tolerance effectively is a challenge --> but they are based on fine-grained updates to a mutable state --> therefore it can only work in 2 ways --> Either we replicate data across the machines or log the updates that we are making.
    - both are expensive and require copying values over cluster network
    
    --> RDDs provide coars grained transformations that apply the same operation TO MANY ITEMS --> Therefore, even if an RDD is lost, we will always have enough information to rebuild just that partition.



- RDDs also accomodate other computing frameworks such as mpareduce, dryarlinq, swl, pregel and haloop


```

### RDDs

```text

- RDD is read only 

```

### Spark Programming Interface

- 