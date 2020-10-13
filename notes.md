
# Compile-time Validation


When the compiler can immediately tell when you make a mistake, it feels like you are working against it.
This creates the fundamental experience that all computer science students are very familiar with.
It feels like banging rocks together.

If I want to build something, first I have to get building blocks.
So I bang rocks together, trying to make them fit together, but all I can do is create a fire.
The fires can be useful, but if I'm not careful, I can accidentally burn down important things around me.
My understanding is very primitive, and all I have is hard work and my ability to learn.

If I keep on banging rocks together, the rocks start to crack and break apart, randomly changing their shape.
They still don't fit together very well, but now their sharp edges cut me instead of starting fires.
I learned enough to not cause fires, and some of the sharp pieces may actually be useful for others.
But my understanding is still primitive.

If I keep on doing this long enough, I can learn to control where the stones crack.
I am no longer just bangig rock together. I am chiseling the stone into whatever I want.
I am no longer starting fires or cutting myself. I am leaving only tiny pebbles and dust behind.
I am no longer bound by the shape of the stone. I can chisel them into building blocks that anyone can use.
My understanding is mature enough to be consistently helpful and productive.

But still, the most complex structure I can build at the largest scale is a pyramid.

> Most software today is very much like an Egyptian pyramid  
> with millions of bricks piled on top of each other,
> with no structural integrity,
> but just done by brute force and thousands of slaves.
> *Alan Kay*


Building Eiffel's tower is impossible this way.
They needed to innovate just to be able to build it.
- tower cranes, that were mounted on the elevators
	- move up as the construction progressed
- portable forges, that heated rivets close to their assembly
	- allowed riveting all the way up the tower

---

SHOW CODE HERE:

sololearn.com/Codes/


### 

Test effort can be reduced by:

- giving context to users and the compiler.
- making invalid states unrepresentable.

How?


### Type Safety

Replace general types with specialized types.

- user name: string -> UserName type
- file path: string -> FilePath type

Can be done with a simple struct wrapper.

!!!


```
code example
```

!!!


### Phantom Types

Differentiate different things within a type.

- numbers with unit of measurement
- FilePath concatenation

Can be done with generics.

!!!


```
code example
```

!!!


- ~~giving context to users and the compiler~~
- making invalid states unrepresentable
	- restrict operations with phantom type tags
	- example: FilePath concatenation

!!!

```
code example
```


!!!


### Summary

- the DRY principle
- make bad things hard
- let the compiler do the work

!!!

### In Practice

- write pure functions
- use types to provide context
- use mathematical abstractions
- aim for functional architecture

!!!


Together they are:

- **functional programming**
- **type-driven development**

!!!


### What is Simplicity

Slightly increasing the complexity of the building blocks  
dramatically improves what can be built.

!!!




!!!


- pits of failure vs pits of success
- quality cannot be "tested into" SW

!!!


### Leadership

- incremental change does not work
- solution requires leadership and technology
- this is a human problem, not a technology problem


!!!

- we need fundamental change
- we need computer scientists


