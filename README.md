# Awesome-Browser-Fuzzing
A curated list of browser fuzzing researches, papers, tools, ...

## [Domato](https://github.com/googleprojectzero/domato)

A DOM Fuzzer by Ivan Fratric from Google project zero

## [FREEDOM](https://github.com/sslab-gatech/freedom)

[FreeDom: Engineering a State-of-the-Art DOM Fuzzer](https://gts3.org/assets/papers/2020/xu:freedom.pdf)] by Georgia Institute of Technology. (https://github.com/sslab-gatech/freedom)

FreeDom, a full-fledged clusterfriendly DOM fuzzer that works with both generative and coverageguided modes. FreeDom relies on a context-aware intermediate
representation to describe HTML documents with proper data dependencies. FreeDom also exhibits up to 3.74× higher throughput
through browser self-termination. FreeDom has found 24 previously unknown bugs in commodity browsers including Safari, Firefox, and Chrome, and 10 CVEs has been assigned so far. With the context-aware generation, FreeDom finds 3× more unique crashes in WebKit than the state-of-the-art DOM fuzzer, Domato. FreeDom guided by coverage is more effective in revealing new code blocks (2.62%) and finds three complex bugs that its generative approach fails to find. However, coverage-guided mutation that bootstraps with an empty corpus triggers 3.8× fewer unique crashes than the generative approach. The newly revealed coverage, more often than not, negatively affects the effectiveness of DOM fuzzers in bug finding. Therefore, we consider context-aware generation the best practice to find more DOM engine bugs and expect further improvement on coverage-guided DOM fuzzing facilitated by FreeDom


## [Minerva](https://github.com/ChijinZ/Minerva)

[Minerva: Browser API Fuzzing with Dynamic Mod-Ref Analysis](https://hexhive.epfl.ch/publications/files/22FSE.pdf)
We propose Minerva, an efficient browser fuzzer for browser API bug detection. The key idea is to leverage API interference relations to reduce redundancy and improve coverage. Minerva consists of two modules: dynamic mod-ref analysis and guided code generation. Before fuzzing starts, the dynamic mod-ref analysis module builds an API interference graph. It first automatically identifies individual browser APIs from the browser’s code base. Next, it instruments the browser to dynamically collect mod-ref relations between APIs. During fuzzing, the guided code generation module synthesizes highly-relevant API invocations guided by the mod-ref relations. We evaluate Minerva on three mainstream browsers, i.e. Safari, FireFox, and Chromium. Compared to state-of-the-art fuzzers, Minerva improves edge coverage by 19.63% to 229.62% and finds 2x to 3x more unique bugs. Minerva has discovered 35 previously-unknown bugs out of which 20 have been fixed with 5 CVEs assigned and acknowledged by browser vendors
