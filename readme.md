Table Of Contents

Overview


Two Feedback Loops:
1.  Inner loop focuses on units of code and what they do.
2.  Outer loop focuses on the organization and the team.  Ensuring that the
application serves the users needs.

**Dislike for testing** comes from the fact that most people do not do as well
with work they find uninspiring.  Few developers enjoy testing their code and
therefore arn't as good at it which then makes it less enjoyable to do because
they're not as good at it.  It's a vicious cycle.

Purposes Of Testing:
*  Drive the quality of implementation (_Does it work?_)
*  Drive the quality of the design (_Is our code well structured?_)
*  What does _well structured_ mean? 

  * **Low coupling** - when one object changes others don't have to change with it.
  * **High cohesion** - objects have a single defined purpose/responsibility.  They
are not trying to do too many things at once.

*  Makes us clarify the acceptance criteria, knowing when we have "completed" a
    feature.
*  Allows us to catch regression error, making it easier to add new features
    with confidence.
*  Adds an executable description of what code does
*  Discourages us from adding functionality on top of what is really required.
*  Makes it easier to refactor.  Developers can then write code that
    communicates its purpose more effectively


---
**Golden Rule of Testing**: Never write new functionality without a failing
test.

___


### Levels of Testing

**Acceptence**: does the whole system work?
**Integration**: does our code work against code we can't change? Like external
libraries
**Unit**: do our objects do the what we expect?  are they a pleasure to work
with?

Unit tests tell us about code quality but don't give us as much confidence about
the system as a whole.  Unit tests need to create the Object, its dependencies,
send messages, and check that the behavior is as expected.  In order for a class
to be easy to unit test it inherently needs to be _loosely coupled_ and _highly
cohesive_.

___

**Bloated Constructor**: when instantiated an object becomes unweilding with the
number of dependencies being injected, look for ways to naturally combine those
dependencies to a higher level of abstraction and then use that abstraction in
the object being tested.
