# CMPS 2200 Recitation 04
## Answers

**Name:**__Srikanya Balaji Garuda_______________________
**Name:**_________________________


Place all written answers from `recitation-04.md` here for easier grading.

- **4) (2 pts)** Assume that a word `w` appears `n` times. What is the **work** and **span** of `word_count_reduce` for this word, assuming a parallel implementation of the `reduce` function?

Work: $O(n)$
Span: $O(\log n)$

- **5) (2 pts)** What is the problem that prevents us from easily parallelizing this solution?

The collect function requires sorting all the key-value pairs to group them together. This sorting step acts as a sequential block because it forces the program to pause and process the data step by step rather than all at once, preventing full parallelization.

