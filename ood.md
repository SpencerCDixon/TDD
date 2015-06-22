Object is an implementation of onr ore more roles; a role is a set of related
responsibiltities; and a responsibility is an obligation to perform a task or
know information.


CRC cards:
Candidate, Responsibilities, Collaborators

Sending Messages:
the calling object should describe what it wants _in terms of the role_ that its
neighbor plays.  AKA "Tell, Don't Ask" AKA Law of Demeter

Objects make decisions based only on the information they hol dinternally or tha
twhich cam ewith the triggering message.  They avoid navigating to other objects
to make things happen.

