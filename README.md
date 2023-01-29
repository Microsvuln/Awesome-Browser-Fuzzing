# Awesome-Browser-Fuzzing
A curated list of browser fuzzing researches, papers, tools, ...

## [Domato](https://github.com/googleprojectzero/domato)

A DOM Fuzzer by Ivan Fratric from Google project zero

## [FREEDOM](https://github.com/sslab-gatech/freedom)

[FreeDom: Engineering a State-of-the-Art DOM Fuzzer](https://gts3.org/assets/papers/2020/xu:freedom.pdf)] (Georgia Institute of Technology)

FreeDom, a full-fledged clusterfriendly DOM fuzzer that works with both generative and coverageguided modes. FreeDom relies on a context-aware intermediate
representation to describe HTML documents with proper data dependencies. FreeDom also exhibits up to 3.74× higher throughput
through browser self-termination. FreeDom has found 24 previously unknown bugs in commodity browsers including Safari, Firefox, and Chrome, and 10 CVEs has been assigned so far. With the context-aware generation, FreeDom finds 3× more unique crashes in WebKit than the state-of-the-art DOM fuzzer, Domato. FreeDom guided by coverage is more effective in revealing new code blocks (2.62%) and finds three complex bugs that its generative approach fails to find. However, coverage-guided mutation that bootstraps with an empty corpus triggers 3.8× fewer unique crashes than the generative approach. The newly revealed coverage, more often than not, negatively affects the effectiveness of DOM fuzzers in bug finding. Therefore, we consider context-aware generation the best practice to find more DOM engine bugs and expect further improvement on coverage-guided DOM fuzzing facilitated by FreeDom
