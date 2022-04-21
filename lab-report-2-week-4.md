# Lab report 2

## Change 1
- Screen shot of changes
![image](https://user-images.githubusercontent.com/59184714/164493416-a0d0d688-022a-4241-b90c-9e960c63e463.png)


- Link to the failure document
https://github.com/Henryfzh/CSE-15L-Markdown-parser/commit/7277c0023d2f7eed91859f0ee361c6d6888206b1

- Symptom of the bug
![image](https://user-images.githubusercontent.com/59184714/164497409-11f6edae-c9df-4089-b440-dfd18cc6b841.png)

- Relation between bugs, the symptom, and the failure-inducing input:
Because there is a missing ")" at the document, the code cannot find the link and get the correct index, so it will generate the problem. When the code cannot find the index of the missing ")", it will have out of bound problem.
