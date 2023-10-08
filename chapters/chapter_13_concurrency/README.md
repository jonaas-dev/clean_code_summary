<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [CHAPTER 13: CONCURRENCY](#chapter-13-concurrency)
  - [Why Concurrency?](#why-concurrency)
  - [Myths and Misconceptions](#myths-and-misconceptions)
  - [Challenges](#challenges)
  - [Concurrency Defense Principles](#concurrency-defense-principles)
  - [Single Responsibility Principle](#single-responsibility-principle)
  - [Corollary: Limit the Scope of Data](#corollary-limit-the-scope-of-data)
  - [Corollary: Use Copies of Data](#corollary-use-copies-of-data)
  - [Corollary: Threads Should Be as Independent as Possible](#corollary-threads-should-be-as-independent-as-possible)
  - [Know Your Library](#know-your-library)
  - [Thread-Safe Collections](#thread-safe-collections)
  - [Know Your Execution Models](#know-your-execution-models)
  - [Producer-Consumer](#producer-consumer)
  - [Readers-Writers](#readers-writers)
  - [Dining Philosophers](#dining-philosophers)
  - [Beware Dependencies Between Synchronized Methods](#beware-dependencies-between-synchronized-methods)
  - [Keep Synchronized Sections Small](#keep-synchronized-sections-small)
  - [Writing Correct Shut-Down Code Is Hard](#writing-correct-shut-down-code-is-hard)
  - [Testing Threaded Code](#testing-threaded-code)
  - [Treat Spurious Failures as Candidate Threading Issues](#treat-spurious-failures-as-candidate-threading-issues)
  - [Get Your Nonthreaded Code Working First](#get-your-nonthreaded-code-working-first)
  - [Make Your Threaded Code Pluggable](#make-your-threaded-code-pluggable)
  - [Make Your Threaded Code Tunabl](#make-your-threaded-code-tunabl)
  - [Run with More Threads Than Processor](#run-with-more-threads-than-processor)
  - [Run on Different Platforms](#run-on-different-platforms)
  - [Instrument Your Code to Try and Force Failures](#instrument-your-code-to-try-and-force-failures)
  - [Hand-Coded](#hand-coded)
  - [Automated](#automated)
  - [Conclusion](#conclusion)
  - [Bibliography](#bibliography)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->




## CHAPTER 13: CONCURRENCY

### Why Concurrency?
### Myths and Misconceptions
### Challenges
### Concurrency Defense Principles
### Single Responsibility Principle
### Corollary: Limit the Scope of Data
### Corollary: Use Copies of Data
### Corollary: Threads Should Be as Independent as Possible
### Know Your Library
### Thread-Safe Collections
### Know Your Execution Models
### Producer-Consumer
### Readers-Writers
### Dining Philosophers
### Beware Dependencies Between Synchronized Methods
### Keep Synchronized Sections Small
### Writing Correct Shut-Down Code Is Hard
### Testing Threaded Code
### Treat Spurious Failures as Candidate Threading Issues
### Get Your Nonthreaded Code Working First
### Make Your Threaded Code Pluggable
### Make Your Threaded Code Tunabl
### Run with More Threads Than Processor
### Run on Different Platforms
### Instrument Your Code to Try and Force Failures
### Hand-Coded
### Automated
### Conclusion
### Bibliography

<!-- ////////////////////////////////////////////////////////  -->
<!-- ////////////////////////////////////////////////////////  -->
<!-- ////////////////////////////////////////////////////////  -->
