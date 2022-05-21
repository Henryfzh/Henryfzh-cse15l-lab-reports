# Lab Report 4

[Link to My Repository ](https://github.com/Henryfzh/CSE-15L-Markdown-parser)

[Link to Peer's Repository](https://github.com/tcarman/markdown-parser)

## Snippet 1:

- MarkdownParseTest:

  ![image](https://user-images.githubusercontent.com/59184714/169658195-57bbb7cd-b190-4744-ba6b-15c9785eb30f.png)
  
  (The snippet1.md document includes the text in Snippet1)

- Expeted Output:

  ![image](https://user-images.githubusercontent.com/59184714/169351285-2967c435-f690-4512-9167-505588f75b45.png)

- My code (Passed):

  ![image](https://user-images.githubusercontent.com/59184714/169345030-a335c388-7e94-4899-b73e-3845b78efed3.png)

- Peer's code (Not Passed):

  ![image](https://user-images.githubusercontent.com/59184714/169347367-d85b7923-4482-4227-946c-7809c02ad4dc.png)
  
  ![image](https://user-images.githubusercontent.com/59184714/169658365-d05c348c-184b-4789-85c9-03500e9ce1c4.png)

  
- I think I do not need to make anychanges to my code, because the output of my code is the same with the expected output.
  
## Snippet 2:

- MarkdownParseTest:

  ![image](https://user-images.githubusercontent.com/59184714/169658638-ee25b5e9-0ccc-40b8-994b-a028213eb674.png)

- Expected Output:

  ![image](https://user-images.githubusercontent.com/59184714/169354054-74121638-cd10-4d1a-b517-fdb71737e548.png)

- My code (Not Passed):

  ![image](https://user-images.githubusercontent.com/59184714/169345723-6d185012-7bd2-4106-b2f9-da4b272d704b.png)
  
  ![image](https://user-images.githubusercontent.com/59184714/169658433-b87ed811-e011-4382-a122-dc54719393d1.png)


- Peer's code (Not Passed):

  ![image](https://user-images.githubusercontent.com/59184714/169347557-2bc50d32-ef0c-4a52-8047-41e7b53aa7e3.png)
  
  ![image](https://user-images.githubusercontent.com/59184714/169658417-6a69dad8-bc98-4054-9c76-9cb38f5636e4.png)


- I think I cannot use a small code to correct the error. I think I need to use a stack to solve this issue, when the code find a "[", put it in the stack whenever it finds the "]" pop them out the stack, and read the information between this two stack. 


## Snippet 3:

- MarkdownParseTest:

  ![image](https://user-images.githubusercontent.com/59184714/169658620-fa00eb6e-771b-4ce2-aae0-acfcb0d960cb.png)

- Expected Output:

  ![image](https://user-images.githubusercontent.com/59184714/169657294-e50d6d19-d14a-4b67-85e8-0dc81b313e14.png)

- My code (Not Passed):

  ![image](https://user-images.githubusercontent.com/59184714/169345842-bde14ab5-5f29-478f-872a-3b56f6148a76.png)
  
  ![image](https://user-images.githubusercontent.com/59184714/169658504-1de8e763-1e3e-4fa2-a212-b25df6fab428.png)

- Peer's code (Not Passed):

  ![image](https://user-images.githubusercontent.com/59184714/169347461-5f40e9ae-2aa7-437e-bed2-0890d0af4201.png)
  
  ![image](https://user-images.githubusercontent.com/59184714/169658526-1e32d37a-aad1-4e72-9cc8-d6d3a78e55c5.png)

  
 - It is also difficult to fix the problem in small code, because I need to fix all the empty space, and I also need to fix the issue that without ")". I think to eliminate the empty space I can make the code to find the non-empty strings. In order to solve without ")", I can make the code to ignore all the content without the ")".
