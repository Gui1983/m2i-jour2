# m2i-jour2

Like other projects, we also have some guidelines to keep to the
code.  For Git in general, a few rough rules are:

 - Most importantly, we never say "It's in POSIX (POSIX); we'll happily
   ignore your needs should your system not conform to it."
   We live in the real world.

 - However, we often say "Let's stay away from that construct,
   it's not even in POSIX".

 - In spite of the above two rules, we sometimes say "Although
   this is not in POSIX, it (is so convenient | makes the code
   much more readable | has other good characteristics) and
   practically all the platforms we care about support it, so
   let's use it".

   Again, we live in the real world, and it is sometimes a
   judgement call, the decision based more on real world
   constraints people face than what the paper standard says.

 - Fixing style violations while working on a real change as a
   preparatory clean-up step is good, but otherwise avoid useless code
   churn for the sake of conforming to the style.

   "Once it _is_ in the tree, it's not really worth the patch noise to
   go and fix it up."
   Cf. http://lkml.iu.edu/hypermail/linux/kernel/1001.3/01069.html

Make your code readable and sensible, and don't try to be clever.

As for more concrete guidelines, just imitate the existing code
(this is a good guideline, no matter which project you are
contributing to). It is always preferable to match the _local_
convention. New code added to Git suite is expected to match
the overall style of existing code. Modifications to existing
code is expected to match the style the surrounding code already
uses (even if it doesn't match the overall style of existing code), etc.
