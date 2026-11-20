# Evaluation Benchmark: Cheese Agent Test Scenarios

This document contains 3 evaluation scenarios designed to test Cheese across its primary roles.

---

## Scenario 1: Programming Tutor Benchmark
- **Context:** Student encountering infinite recursion on a binary tree height function.
- **Input:**
  > *"I'm getting a `RecursionError: maximum recursion depth exceeded` on my binary tree height function in Python. Why is this happening?"*
  > ```python
  > def tree_height(node):
  >     if node is None:
  >         return 0
  >     left_height = tree_height(node)
  >     right_height = tree_height(node.right)
  >     return 1 + max(left_height, right_height)
  > ```
- **Expected Behavior:**
  1. No immediate code rewrite.
  2. Onion / shrinking problem analogy.
  3. Step-by-step trace showing `node` passed repeatedly without `.left`.
  4. Socratic inquiry pointing directly to line 4.

---

## Scenario 2: Personal Coach Benchmark
- **Context:** Student frozen with a 72-hour deadline on an OS C shell project.
- **Input:**
  > *"I have an OS assignment building a basic UNIX shell in C due in 72 hours. I haven't written a single line of code because every time I open the spec sheet I feel stupid and overwhelmed by `fork()`, `execvp()`, `waitpid()`, and signal handling. I just end up doomscrolling."*
- **Expected Behavior:**
  1. Zero judgment; neutralizes imposter syndrome.
  2. 5-phase breakdown over 72 hours.
  3. Single 25-minute immediate challenge: `while(1)` REPL loop with `fgets()`.

---

## Scenario 3: Research Agent Benchmark
- **Context:** Evaluating gRPC vs. REST for an internal microservice.
- **Input:**
  > *"For my web services course final project, our team is building an internal microservice that handles user notifications and events. Should we use REST over HTTP/1.1 or gRPC over HTTP/2? Give us a structured comparison and a clear recommendation."*
- **Expected Behavior:**
  1. Markdown table comparing serialization, transport, contracts, tooling, and streaming.
  2. Concrete criteria-based recommendations.
