# My Working Philosophy

## My Process
  1.  **Understand the problem:** This is always the first step. Without defining & understanding the problem or goal it's difficult to evaluate any potential solution. 
  -  How will we know we succeeded?
  -  What are the critical use cases & edge cases? 
  -  What are the most important aspects of the solution? Performance, observability, readability...etc. 
  -  What are the existing systems/structures/components that we need to interact with?
  2. **Make a Plan**
  -  The scope of the plan depends mostly on the complexity of the changes & number of moving/interconnected components. 
  -  The main goal is to find unknowns early on which may mean my changes won't work
  3. **Get it working Simply:** 
  -  It is easy to for our brains to jump to optimizations prematurely, this tends to lead to unnecessary complexity
  -  Getting the simplest solution working first will make it easier & safer to optimize incrementally
  -  Fast Feedback. I want to know that the changes I'm making are having the intended effect as quickly as possible. This can mean anything from reloading a page to running unit tests on save.
  -  Integrate components early on. The way in which components interact has been the biggest source of late risk realization for me in the past. Integrating these pieces first tends to surface risk sooner  e.g. frontend to api, internal api to external api...etc.
  4. **Refactor**
  -  Surrounding working pieces with tests before refactoring helps ensure I haven't broken anything
  -  Evaluate what I have against my design philosophy & make changes as needed

## My Design Philosophy

- **Simplicity**
  - 
- **YAGNI (You ain't gonna need it)**
  - As engineers it can be easy to get ahead of ourselves & solve problems that don't exist yet (and may not ever exist)
  - This includes abstractions
- **Readability**
- **Data-Oriented**

## Practices

- Take time to Learn
  - understand tools, technologies

## Communicating with others

- Ask Questions
