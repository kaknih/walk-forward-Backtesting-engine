This project is a lightweight backtesting engine I created to test trading ideas while respecting how time works in real markets. Instead of using shuffled data or overly optimistic assumptions, it employs a walk-forward setup. Every decision relies on information that would have been available at that moment. Signals are lagged, so positions are based on yesterday’s data and applied to today’s returns. This approach helps avoid lookahead bias and unrealistic performance.

To ensure honest results, the framework compares a simple moving-average crossover strategy against basic but important benchmarks, including buy-and-hold and a random long/cash strategy. This makes it easier to determine whether a strategy is meaningful or just benefiting from random fluctuations. I also included a small parameter sweep across different MA windows to test how sensitive the results are, rather than depending on a single chosen configuration.

The goal of this project isn’t to provide a profitable trading system, but to create a clean evaluation tool that makes it harder to mislead yourself when testing ideas. It aims to serve as a foundation for further experimentation, where factors like transaction costs, risk controls, or alternative signals can be added and assessed under more realistic conditions.

Note: Code comments were generated with AI assistance.
