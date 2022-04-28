# Lab report 2

## Change 1
- Screen shot of changes
![image](https://user-images.githubusercontent.com/59184714/164493416-a0d0d688-022a-4241-b90c-9e960c63e463.png)


- Link to the failure document:[Failure Case 1](https://github.com/Henryfzh/CSE-15L-Markdown-parser/commit/7277c0023d2f7eed91859f0ee361c6d6888206b1)

- Symptom of the bug
![image](https://user-images.githubusercontent.com/59184714/164497409-11f6edae-c9df-4089-b440-dfd18cc6b841.png)

- Relation between bugs, the symptom, and the failure-inducing input:
Because there is a missing ")" at the document, the code cannot find the link and get the correct index, so it will generate the problem. When the code cannot find the index of the missing ")", it will have out of bound problem. My failure-inducing input is "[Link2](some-thing.html" with missing ")" at the end of the line, so it will have an error.

## Change 2
- Screen shot of changes
![image](https://user-images.githubusercontent.com/59184714/164566551-433e03bd-8447-4f4c-bb67-eb32803528f1.png)

- Link to the failure document:[Failure Case 2](https://github.com/Henryfzh/CSE-15L-Markdown-parser/commit/21d95402730b00f7734697639fb163bd345ad035#diff-c30dbff4e529133282d848da192ac83e5d6f1c7593c0e31db0e4104f43178d3e)
- Symptom of the bug:
When there is an empty line at the end of the markdown document, the program will keep running without ending. 
![image](https://user-images.githubusercontent.com/59184714/164566955-b38c2063-1cef-4f6c-8200-12e3dec8d520.png)

- Relation between bugs, the symptom, and the failure-inducing input:
My failure-inducing input is to add an empty line at the end of the document, and it won't stop. Because the code was looking for the backets, but there is no at the end of the document. When it will not stop running until it finds another backet.

## Change 3
- Screen shot of changes
![image](https://user-images.githubusercontent.com/59184714/164507658-f7ac39d3-43f3-4fa2-a2cd-029dab922804.png)

- Link to the failure document:[Failure Case 3](https://github.com/Henryfzh/CSE-15L-Markdown-parser/commit/c9e1964cf3651656aa5fcf9dbf693932aece33be)

- Symptom of the bug:
Nothing will be included in the output, because the code cannot find the link inside the backets. Only a comma in the output, but it is false
![image](https://user-images.githubusercontent.com/59184714/164509063-3f3214b4-1c9a-4d39-91d1-5243de8c66fe.png)


- Relation between bugs, the symptom, and the failure-inducing input:
The original code cannot find the empty link and it just keep output an empty string, that's why the output is empty. My failure-inducing input dose not include any links in the document, so the output is like " , ", but it makes no sense.
