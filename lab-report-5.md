# **LAB REPORT 5 - Debugging Scenario**

## **PART 1 - EDSTEM THREAD 06/05/2023**

### **Anonymous Student:**

**Title** : Bubble Sort Debugging 

**What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?**

VS Code on Macbook

**Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead.
Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.**

I have written the bubble sort algorithm. When I run the JUnit test, it fails. I cannot understand where the bug is in the algorithm. 
The expected output is that all tests have passed. The actual output is that one test has failed.
This is the error message shown -

```
arrays first differed at element [0]; expected:[1] but was:[3]
 at SortTester.sortTest1(SortTester.java:11)
Caused by: java.lang.AssertionError: expected:[1] but was:[3]
```

I am providing screenshots of my code and output below:

![Image](FaultyBubbleSort.png)

![Image](BashRunScript.png)

![Image](TerminalErrorJUNIT.png)

![Image](FaultySortTester.png)


**Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.**

The failure inducing input was the array : ``int[]{3,7,2,1,8,1,9}``. The bubble sorting algorithm should return the sorted output as ``{1,1,2,3,7,8,9}``.

---
### **Helpful TA:**

Thank you for providing good context and detail to allow me to help you. 
What I would say is make sure you are **swapping array elements properly**

---
### **Anonymous Student:**

Thank you very much for your suggestion. I realized that I was assigning the value of ``arr[j-1]`` to both the temporary ``temp`` variable and ``arr[j]``. This resulted in the loss of the element at ``arr[j]`` and duplicated ``arr[j-1]``
