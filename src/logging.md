

# StLog

Ultra lightweight logging framework for resource constrained devices


* O(1) execution time. Logging a message of arbitrary size is done in a constant number of instructions.

* O(0) memory usage. The messages are NOT stored in the target device memory.

* Supports different logging levels: error, warning, info, debug and trace, in decreasing level of severity. By default, the dev profile logs debug, and more severe, messages and the release profile logs info, and more severe, messages, but this can changed using the Cargo features of this crate.

* Provides a global logging mode


<https://crates.io/crates/stlog>

<https://japaric.github.io/stlog/stlog/>


Decoded with

<https://crates.io/crates/stcat>
