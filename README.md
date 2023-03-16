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

This error message is typically generated when it can't find a type annotation or stub for the module "cv2". The "cv2" module is typically used for computer vision tasks in Python and requires the OpenCV library to be installed.To resolve this error, you should ensure that the OpenCV library is installed on your system and that your Python environment can find it. You should also make sure that you have installed any necessary dependencies for the "cv2" module.If you have already installed OpenCV and its dependencies, you may need to create a stub file for "cv2" module, which provides type hints for the functions and classes defined in the module.

error: Library stubs not installed for "PIL"

This error message is generated when it can't find the type annotations or stub files for the "PIL" module. "PIL" stands for Python Imaging Library, which is a popular library used for image processing tasks in Python. To resolve this error, you can install the type stubs for "PIL" by running the following command:

pip install pillow-stubs

3) https://github.com/Abhishek010397/Read-Files-Python.git

![image](https://user-images.githubusercontent.com/82575404/225572841-d2ece2fd-5872-4586-b8cc-2886beb7f8ca.png)

 error: Incompatible types in assignment (expression has type "TextIOWrapper", variable has type "str")
 
 This error message is generated when you're trying to assign a value of one type to a variable of a different type. Specifically, the error message "Incompatible types in assignment (expression has type 'TextIOWrapper', variable has type 'str')" means that you're trying to assign a "TextIOWrapper" object to a variable that is declared as a "str" type.A "TextIOWrapper" object is a file-like object that is returned when you open a file in text mode using the built-in "open" function in Python. On the other hand, a "str" type variable is a string variable.To fix this error, you need to make sure that you're assigning the correct type of value to your variable. If you want to assign the contents of a file to a string variable, you need to read the contents of the file using the "read" method on the "TextIOWrapper" object.

NOTE- To get detailed Static Analysis we can use Pylint. It also gives us code rating based on errors.

For eg 3, using pylint

![image](https://user-images.githubusercontent.com/82575404/225575181-0272ffb2-c681-48d9-ae6c-92a69a355e4d.png)



