# [Tim Bradshaw](https://tfeb.org/)
## Note
No code will change in my permanent GitHub repos after August, 2025, as I am moving away from GitHub.  Everything mentioned in this document has now been migrated: the repos still exist on GitHub but only as archives.  Some other smaller things (not mentioned here) will move in due course.  Here are the new locations:

- [**Index page**](https://tfeb.org/computer)
- [**Documentation index page**](https://tfeb.org/fragments/documentation/) (the new version of this document)
- [**Git repos**](https://tfeb.org/computer/repos/)

See also [Minimum clown](https://tfeb.org/fragments/2025/08/26/minimum-clown/) which explains why I've done this, if it's not obvious.

---

Some things I have made.

## Larger things
Some of which are merely piles of smaller things, related largely by their shared history and authorship.  There should generally be some documentation and infrastructure to build and install things here.  [Some notes on what goes where](what-goes-where.md), probably only interesting to me.

### xkcd-936: random passphrases
**\[Migrated]** Based on [xkcd 936](https://www.xkcd.com/936/).  Python 2.7 or 3.  [Documentation](https://tfeb.org/fragments/documentation/xkcd-936.html) / [Source code](https://tfeb.org/computer/repos/xkcd-936.git).

### Warranted commands
**\[Migrated]** MacOS now has protections which are completely orthogonal to the traditional Unix file access controls.  These can make running unattended periodic tasks difficult.  A solution is to have a single program which you 'bless' with full disk access and which can then run other things.  To make this not insanely dangerous that program should allow you to specify what it will, and won't run.  That's what `warranted` is: a tool like `sudo` but without the implication of access as another user, and with a better (I think) configuration syntax.  It's written in [Racket](https://racket-lang.org/), and you'll need a Racket installation to build it.

[Documentation](https://tfeb.org/fragments/documentation/warranted.html) / [Source code](https://tfeb.org/computer/repos/warranted.git)

### Conduit packages for Common Lisp
**\[Migrated]** Conduit packages are packages which serve as conduits for one or more underlying packages: they let you make a system which consists of several implementation packages available through one package, or to provide packages which extend other packages, or replace some symbols they export with symbols from a different package.

[Documentation](https://tfeb.org/fragments/documentation/conduit-packages.html) / [Source code](https://tfeb.org/computer/repos/conduit-packages.git)

### Destructuring match for Common Lisp
**\[Migrated]** `destructuring-match` is a construct which is like a combination of `case` and a slightly extended `destructuring-bind`.  It is extremely useful for writing macros.

[Documentation](https://tfeb.org/fragments/documentation/dsm.html) / [Source code](https://tfeb.org/computer/repos/dsm.git)

### Štar: an iteration construct for Common Lisp
**\[Migrated]** Štar is a concise and extensible iteration construct for Common Lisp which aims to be pleasant to use, easy to understand, fast if needed, general, and not to look like Fortran.

[Documentation](https://tfeb.org/fragments/documentation/star.html) / [Source code](https://tfeb.org/computer/repos/star.git)

### Some Common Lisp tools
**\[Migrated]** A collection of fairly miscellaneous Common Lisp tools which I use to help with program construction and management, which I have written over the years in order to generally get stuff done.  Slowly growing as I unearth things and publish them.

[Documentation](https://tfeb.org/fragments/documentation/tfeb-lisp-tools.html) / [Source code](https://tfeb.org/computer/repos/tfeb-lisp-tools.git)

### Some Common Lisp hacks
**\[Migrated]** A collection of small Common Lisp hacks, which may be useful in programs, and which I've written over the last thirty-odd years.  Some of them are genuinely useful, some of them are little more than toys written long ago to prove a point on `comp.lang.lisp`.  They are largely independent of each other.

[Documentation](https://tfeb.org/fragments/documentation/tfeb-lisp-hax.html) / [Source code](https://tfeb.org/computer/repos/tfeb-lisp-hax.git)

### Symbol nicknames
**\[Migrated]** Symbol nicknames is a toy which allows you to have multiple names resolving to the same symbol, which may or may not be useful.  This is implementation-specific as it requires hooking symbol lookup: it is fully supported in LispWorks and SBCL, while the core should be portable CL.  It's never going to be more than a toy.

[Documentation](https://tfeb.org/fragments/documentation/symbol-nicknames.html) / [Source code](https://tfeb.org/computer/repos/symbol-nicknames.git)

### Some Common Lisp implementation-specific hacks
**\[Migrated]** Some things which I've written which depend on specific implementations of CL that I use or have used.  Currently not much has been added but I will probably add more over time.  Some of this code may work, some of it may once have worked, some of it may never have worked: *caveat emptor*.

[Documentation](https://tfeb.org/fragments/documentation/tfeb-lisp-implementation-hax.html) / [Source code](https://tfeb.org/computer/repos/tfeb-lisp-implementation-hax.git)

## Smaller things
Shards and fragments which may be interesting to someone.

### Some Common Lisp toys
**\[Migrated]** A collection of Common Lisp toys: some may work, some may not work, some may never have worked.

[Documentation](https://tfeb.org/fragments/documentation/tfeb-lisp-toys.html) / [Source code](https://tfeb.org/computer/repos/tfeb-lisp-toys.git)

### A toy Lisp reader: reeder
**\[Migrated]** Reeder is a toy table-driven Lisp reader, written in Common Lisp.  I wrote it mostly to see how hard it would be.  It is a toy, it probably has bugs and it may be hard to build if you are not me.  But it is extensible and configurable.

[Documentation](https://tfeb.org/fragments/documentation/reeder.html) / [Source code](https://tfeb.org/computer/repos/reeder.git)

### A toy for playing with λ-calculus: oa
**\[Migrated]** Oa – one argument – is a toy [Racket](https://racket-lang.org/) language for playing with  λ-calculus.  In fact there are a total of four languages:

- a pure single-argument normal-order language where functions are written as, for instance `(λ x x)`;
- a fancy version of the above language where you can write `(λ (x y) x)` which is turned into `(λ x (λ y x))`, and where `(f a b)` is turned into `((f a) b)`;
- a pure single-argument applicative-order language;
- a fancy version of the applicative language.

I wrote oa to learn about implementing languages in Racket, and to play with λ-calculus.  I am not convinced the normal-order languages are correct – they certainly used not to be although they seem to be working now.

[Documentation](https://tfeb.org/fragments/documentation/oa.html) / [Source code](https://tfeb.org/computer/repos/oa.git)

## Relics
Artifacts from a past I am forgetting.

(None yet.)

---

[Some other things I have made](https://www.tfeb.org/).
