  CookieJar - A contestant's algorithm toolbox (go)
=====================================================

CookieJar is a small collection of common algorithms and data structures that were deemed handy for computing competitions at one point or another. The goal of the toolbox is twofold: to provide some constructs out of the box - if they happen to be applicable - and as a reference collection of the things one should know.

Note, this toolbox was not designed for production work. It is a work in progress and most probably will always remain such. It may be lacking, it may be buggy and it may change drastically between commits (although every effort is made not to). You're welcome to use it, but it's your head on the line :)

  Contents
------------

Algorithms:
 - Work in progress

Data Structures:
 - [Bag](http://godoc.org/github.com/karalabe/cookiejar/bag)
 - [Deque](http://godoc.org/github.com/karalabe/cookiejar/deque)
 - [Priority Queue](http://godoc.org/github.com/karalabe/cookiejar/prque)
 - [Queue](http://godoc.org/github.com/karalabe/cookiejar/queue)
 - [Set](http://godoc.org/github.com/karalabe/cookiejar/set)
 - [Stack](http://godoc.org/github.com/karalabe/cookiejar/stack)

  Performance
---------------

Intel(R) Core(TM) i7-2600 CPU @ 3.40GHz:
```
- bag
    - BenchmarkInsert    309     ns/op
    - BenchmarkRemove    197     ns/op
    - BenchmarkDo        28.1    ns/op
- deque
    - BenchmarkPush      25.4    ns/op
    - BenchmarkPop       6.72    ns/op
- prque
    - BenchmarkPush      171     ns/op
    - BenchmarkPop       947     ns/op
- queue
    - BenchmarkPush      23.0    ns/op
    - BenchmarkPop       5.92    ns/op
- set
    - BenchmarkInsert    259     ns/op
    - BenchmarkRemove    115     ns/op
    - BenchmarkDo        20.9    ns/op
- stack
    - BenchmarkPush      16.4    ns/op
    - BenchmarkPop       6.45    ns/op
```
