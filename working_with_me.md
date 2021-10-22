# My Working Philosophy

## Communicating with others

- We can all learn from each other, regardless of past experience. I try to be curious when others have a different perspective. Seek to understand by asking questions. 
- I try to use neutral language to avoid being critical. Frame things as problems to solve together
- The times I have grown most have come from pairing with people. Getting to see their thought process, not just their solution, but how they go about solving problems.
- Alignment on the goal & what aspects of a solution are important often make communication smoother.

## Communicating with me

- I enjoy pairing to work through obstacles or designs. I prefer hopping on a quick call over a long series of slack messages.

## My Process
  1.  **Understand the problem:** This is always the first step. Without defining & understanding the problem or goal it's difficult to evaluate any potential solution. 
  -  How will we know we succeeded?
  -  What are the critical use cases & edge cases? 
  -  What are the most important aspects of the solution? Performance, observability, readability...etc. 
  -  What are the existing systems/structures/components that we need to interact with? What do responsibilities/concerns belong?
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

- [**Simplicity**](https://www.youtube.com/watch?v=LKtk3HCgTa8)
  - Units of code (methods, interfaces...etc.) which do 1 thing are usually more flexible (decoupled from other code) & easier to understand
  - Complexity means multiple concerns/responsibilities intertwined together
- **YAGNI (You ain't gonna need it)**
  - As engineers it can be easy to get ahead of ourselves & solve problems that don't exist yet (and may not ever exist)
  - This includes abstractions. Abstract & generalize when there is a benefit to doing so and not before.
- [**Readability**](https://medium.com/@egonelbre/psychology-of-code-readability-d23b1ff1258a)
  - Code is read many more times than it is updated, often by someone who has less context than the person who wrote it.
  - Code which is difficult to understand is easy to break

## Practices

- **Take time**
  - Seek to understand tradeoffs instead of searching for a "right" or familiar solution. It takes time to evaluate different solutions & understand what is best in the current context
  - Seek to understand deeply. A deeper understanding helps to simplify problems. A cursory understanding can lead to forcing a sub-optimal solution. This applies to problems, tools, technologies...
  - Important problems take time
- [**Growth mindset**](https://www.brainpickings.org/2014/01/29/carol-dweck-mindset/)
  - Everyone makes mistakes. Mistakes are opportunities to learn. Favor process changes over relying on willpower (or "remembering next time")
- **Incremental Releases**
  - Big Bang releases (releasing a large feature all at once) are often the most risky
  - Releasing changes which are deactivated or invisible to users in production gives feedback earlier & surfaces problems sooner in the development process
  - There's almost always a way to release incrementally (i.e. use feature flags)
