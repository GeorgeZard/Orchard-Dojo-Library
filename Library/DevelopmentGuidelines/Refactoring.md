# Rules of Thumb for Refactoring



Consider [refactoring](http://en.wikipedia.org/wiki/Refactoring) in these cases:

- When a class’s net length is above 300 lines
- If the number of injected dependencies (services) exceeds 5
- It adds invaluable safety if you have unit tests for the code being refactored. If you don't have unit tests for a piece of code, before heavy refactoring is probably the good time to create them.