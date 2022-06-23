# [Tim Bradshaw](https://github.com/tfeb)
Some things I have made.

## Larger things
Some of which are merely piles of smaller things, related largely by their shared history and authorship.  There should generally be some documentation and infrastructure to build and install things here.  [Some notes on what goes where](what-goes-where.md), probably only interesting to me.

### xkcd-936: random passphrases
Based on [xkcd 936](https://www.xkcd.com/936/).  Python 2.7 or 3.  [Documentation](xkcd-936/) / [Source code](https://github.com/tfeb/xkcd-936).

### Warranted commands
MacOS now has protections which are completely orthogonal to the traditional Unix file access controls.  These can make running unattended periodic tasks difficult.  A solution is to have a single program which you 'bless' with full disk access and which can then run other things.  To make this not insanely dangerous that program should allow you to specify what it will, and won't run.  That's what `warranted` is: a tool like `sudo` but without the implication of access as another user, and with a better (I think) configuration syntax.  It's written in [Racket](https://racket-lang.org/), and you'll need a Racket installation to build it.

[Documentation](warranted/) / [Source code](https://github.com/tfeb/warranted)

### Conduit packages for Common Lisp
Conduit packages are packages which serve as conduits for one or more underlying packages: they let you make a system which consists of several implementation packages available through one package, or to provide packages which extend other packages, or replace some symbols they export with symbols from a different package.

[Documentation](conduit-packages/) / [Source code](https://github.com/tfeb/conduit-packages)

### Some Common Lisp tools
A collection of fairly miscellaneous Common Lisp tools which I use to help with program construction and management, which I have written over the years in order to generally get stuff done.  Slowly growing as I unearth things and publish them.

[Documentation](tfeb-lisp-tools/) / [Source code](https://github.com/tfeb/tfeb-lisp-tools)

### Some Common Lisp hacks
A collection of small Common Lisp hacks, which may be useful in programs, and which I've written over the last thirty-odd years.  Some of them are genuinely useful, some of them are little more than toys written long ago to prove a point on `comp.lang.lisp`.  They are largely independent of each other.

[Documentation](tfeb-lisp-hax/) / [Source code](https://github.com/tfeb/tfeb-lisp-hax)

### Some Common Lisp implementation-specific hacks
Some things which I've written which depend on specific implementations of CL that I use or have used.  Currently not much has been added but I will probably add more over time.  Some of this code may work, some of it may once have worked, some of it may never have worked: *caveat emptor*.

[Documentation](tfeb-lisp-implementation-hax/) / [Source code](https://github.com/tfeb/tfeb-lisp-implementation-hax)

## Smaller things
Shards and fragments which may be interesting to someone.

### Some Common Lisp toys
A collection of Common Lisp toys: some may work, some may not work, some may never have worked.

[Documentation](tfeb-lisp-toys/) / [Source code](https://github.com/tfeb/tfeb-lisp-toys)

### A toy Lisp reader: reeder
Reeder is a toy table-driven Lisp reader, written in Common Lisp.  I wrote it mostly to see how hard it would be.  It is a toy, it probably has bugs and it may be hard to build if you are not me.  But it is extensible and configurable.

[Documentation](reeder/) / [Source code](https://github.com/tfeb/reeder)

### A toy for playing with λ-calculus: oa
Oa – one argument – is a toy [Racket](https://racket-lang.org/) language for playing with  λ-calculus.  In fact there are a total of four languages:

- a pure single-argument normal-order language where functions are written as, for instance `(λ x x)`;
- a fancy version of the above language where you can write `(λ (x y) x)` which is turned into `(λ x (λ y x))`, and where `(f a b)` is turned into `((f a) b)`;
- a pure single-argument applicative-order language;
- a fancy version of the applicative language.

I wrote oa to learn about implementing languages in Racket, and to play with λ-calculus.  I am not convinced the normal-order languages are correct – they certainly used not to be although they seem to be working now.

[Documentation](oa/) / [Source code](https://github.com/tfeb/oa)

## Relics
Artifacts from a past I am forgetting.

(None yet.)

---

[Some other things I have made](https://www.tfeb.org/).
