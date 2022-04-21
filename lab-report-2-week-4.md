# Lab report 2

## Change 1
- Screen shot of changes
![image](https://user-images.githubusercontent.com/59184714/164493416-a0d0d688-022a-4241-b90c-9e960c63e463.png)


- Link to the failure document
https://github.com/Henryfzh/CSE-15L-Markdown-parser/commit/7277c0023d2f7eed91859f0ee361c6d6888206b1

- Symptom of the bug
![image](https://user-images.githubusercontent.com/59184714/164497409-11f6edae-c9df-4089-b440-dfd18cc6b841.png)

- Relation between bugs, the symptom, and the failure-inducing input:
Because there is a missing ")" at the document, the code cannot find the link and get the correct index, so it will generate the problem. When the code cannot find the index of the missing ")", it will have out of bound problem. My failure-inducing input is "[Link2](some-thing.html" with missing ")" at the end of the line, so it will have an error.

## Change 2
- Screen shot of changes
- Link to the failure document
- Symptom of the bug
- Relation between bugs, the symptom, and the failure-inducing input:

## Change 3
- Screen shot of changes
![image](https://user-images.githubusercontent.com/59184714/164507658-f7ac39d3-43f3-4fa2-a2cd-029dab922804.png)

- Link to the failure document
https://github.com/Henryfzh/CSE-15L-Markdown-parser/commit/c9e1964cf3651656aa5fcf9dbf693932aece33be

- Symptom of the bug
Nothing will be included in the output, because the code cannot find the link inside the backets. Only a comma in the output, but it is false

- Relation between bugs, the symptom, and the failure-inducing input:
The original code cannot find the empty link and it just keep output an empty string, that's why the output is empty. My failure-inducing input dose not include any links in the document, so the output is like " , ", but it makes no sense.
