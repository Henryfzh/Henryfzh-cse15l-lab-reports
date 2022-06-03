# Lab Report 5

## Difference between results
- [link to the test file ](https://github.com/Henryfzh/CSE-15L-Markdown-parser/tree/main/test-files)

- I chose 473.md and 488.md in the test-files. I used the command bash script.sh to generate two results.txt files and then I used vimdiff to check the difference between two results document

    ![image](https://user-images.githubusercontent.com/59184714/171757276-f25b3f31-f41e-4984-837f-4845ef5fb736.png)
    
 - My test result:
 
    ![image](https://user-images.githubusercontent.com/59184714/171757377-fd88686b-2eb6-4ea5-b650-7c5adda86eae.png)
  
 - Markdown-Parse test result:
 
    ![image](https://user-images.githubusercontent.com/59184714/171757445-560cb4fe-5539-4bd7-80d2-c60a919514d8.png)
    
 - Expected result:
  
    ![image](https://user-images.githubusercontent.com/59184714/171758669-85883a53-e9ef-4220-ae64-70295021ee0f.png)

 - Conclusion: according to the expected result, the first test "[link](foo(and(bar))" should not be a valid link. My code did not work well on this test, and the markdown-parse code worked well on it. However, on the second test "[link] (</my uri>)", the expected result should be a valid link. My code worked well on it but not the markdown-parse code. The reason of my code did not work on the first test because my code can only find the "(" and ")", but not to find out if they are in pairs or they are valid. Below is the piece of the code should be fixed. It should not only simply find "(" and ")", instead, I should create a stack if it finds a "(" then add it to the stack. If it finds ")" then pop one "(" out. After the while loop is done, if there is no "(" or ")" left in the stack, then that is a valid html.

![image](https://user-images.githubusercontent.com/59184714/171759767-10c0235b-cd93-4790-8de2-b97bf7559e3c.png)

