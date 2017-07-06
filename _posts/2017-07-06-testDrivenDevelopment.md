---
layout:            post
title:             "Test Driven Development"
menutitle:         "Test Driven Development"
author:            Prakhar Mathur
tags:              
---

Test Driven Development is an approach for software development using which we need to write tests before the implementation of a particular module. This arises a lot of questions like why to write test first before even knowing what will be the implementation and how can any one know the design of the project before hand. I will try and address these questions in the article to the best of my knowledge.

So, the core idea behind TDD is to know about the specifications first and then implement them. If we know the specifications then we can write tests for them and then we can implement the function according to the requirement of the specification. We all face the problem of a mismatch between the expected behaviour of the application and the resulting behaviour. TDD can help us a lot in solving this problem via testing every single possible module of our code, thus making sure that it performs the way we intended it to and handles all the corner cases.

Now the question arises that why we need to test each and every single module that doesn’t even seem to be relavent enough? There is a famous story of a ship that sank because of a malfunction of a very small unit which was neglected by all, the crew tested every unit except the one that lead to the sinking of the ship. Similarly each and every small module of our code can create a huge impact on the behaviour of our code. But why do we need small modules to test ? What’s the problem in testing bigger modules?  The reason behind testing small modules is cognitive overload. We cannot compute the whole code in our brain. If we were able to do so then there was no need of computer at all but as we can’t process the the whole code at once we need help of automation. When a module gets broken we look at which tests are failing and we can refactor that code easily as we can process it in our brain since our brain can easily calculate the output of a single line of code instead of processing complex code.

Softwares developed using TDD have much better design as we need to test everything, we will modularise our code accordingly, also it will have lesser duplication and fewer edge cases that are not thought through.

Methodology of TDD is simple, all you need to is follow a cycle i.e. Red, Green, Commit, Refactor, Commit. Red means you need to fail the test first i.e. you will write the test so as to clear the specification but you will not implement the function so the test will fail. Green means to pass the test with simple most code which just doesn’t break the contract then we will commit the code. After this we refactor the code in the best possible way and ensuring that the contract is still not broken and on passing the test we commit the final code.

Hopefully now you have a better idea about why we use test driven development as it is evident that it is one of the best ways to make our code maintainable, reusable and non resistant to change.

Best of luck.
