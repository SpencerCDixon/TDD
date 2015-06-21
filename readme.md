Table Of Contents

Overview


Two Feedback Loops:
1.  Inner loop focuses on units of code and what they do.
2.  Outer loop focuses on the organization and the team.  Ensuring that the
application serves the users needs.

* Testing allows us to catch regression errors, making it easier to add new
    features with confidence knowing that we didn't break some other part of the
    system.

**Dislike for testing** comes from the fact that most people do not do as well
with work they find uninspiring.  Few developers enjoy testing their code and
therefore arn't as good at it which then makes it less enjoyable to do because
they're not as good at it.  It's a vicious cycle.

Purposes Of Testing:
*  Drive the quality of implementation (_Does it work?_)
*  Drive the quality of the design (_Is our code well structured?_)
*  What does _well structured_ mean? 

1. **Low coupling** - when one object changes others don't have to change with it.
2. **High cohesion** - objects have a single defined purpose/responsibility.  They
are not trying to do too many things at once.

*  Makes us clarify the acceptance criteria, knowing when we have "completed" a
    feature.
*  Adds an executable description of what code does
*  Discourages us from adding functionality on top of what is really required.


---
**Golden Rule of Testing**: Never write new functionality without a failing
test.
---
