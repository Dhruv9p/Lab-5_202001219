# Lab-5_202001219

Static Analysis:
Static analysis is a method of examining the source code of a software program without executing it. Static analysis can help detect errors, bugs, vulnerabilities, and other quality issues in the code. Static analysis tools can perform various tasks such as checking syntax, style, logic, data flow, control flow, and security. Static analysis can improve the reliability, performance, and maintainability of software by identifying and correcting defects early in the development process.

Static Analysis Tools:

Python:

● Mypy
● Pylint
● Pyflakes
● Pycodestyle (pep8)
● Flake8
● Prospector
● Bandit

Java:

● FindBugs
● PMD
● Checkstyle
● Error Prone
● Spoon
● Spotbugs

Here I am using Mypy for Python.

First I installed mypy in my PC as python was already installed.

![image](https://user-images.githubusercontent.com/82575404/225563133-6ba37e46-c38b-4049-b881-e44df8784db9.png)

Now I have to analyze different python files from github.
Here are some Examples-

1) https://github.com/yjg30737/python-file-shuffle.git

![image](https://user-images.githubusercontent.com/82575404/225567936-617244b9-ce7c-4c80-8f63-42d084f9ddbf.png)

Here no errors were identified.

2) https://github.com/Vaibhav-Mehta-19/automated-attendance-system-using-face-recognition.git

![image](https://user-images.githubusercontent.com/82575404/225568937-e99d0b57-c682-4627-916a-9545c17839c1.png)

error: Cannot find implementation or library stub for module named "cv2"

error: Library stubs not installed for "PIL"

3) https://github.com/Abhishek010397/Read-Files-Python.git

![image](https://user-images.githubusercontent.com/82575404/225572841-d2ece2fd-5872-4586-b8cc-2886beb7f8ca.png)

 error: Incompatible types in assignment (expression has type "TextIOWrapper", variable has type "str")




