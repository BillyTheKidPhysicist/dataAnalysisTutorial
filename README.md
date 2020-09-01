# dataAnalysisTutorial
Quick tutorial on data analysis for my students
makeData.pynb is how the sample data is made. analyzeData.ipynb is the data being analyzed. They both contain helpful information


I will give a quick rundown on why everyone should use python and answer some questions.

Why use python as a physicist???

First, python is very popular and many other physicists use it. It is very easy to find libraries that work in python for a huge variety of tasks including hardware control

Second, the alternatives kind of suck. Controlling hardware with LabView is awful. Image that you didn't know how to read, so you could only listen to things to learn. Well that would get you pretty far, but obviously knowing how to read is a far superior way to learn. 

Python is knowing how to read, LabView is not knowing how to read. It's easier to get started with LabView, but it quickly become horrible because of compatibility issues, you are programming in 2D, and there are not good standards on how to write and comment it.
I'm not a LabView expert, but that is my understanding.

Third, what you can do in Mathematica you can do in Python but it will make sense and it will be readable because it is a 'real' language. The primary library to use in this space is Sympy. Mathematica is definitely more powerful and can solve more problems, but 98 \% of the time Sympy does what I 

Fourth, Python is beautiful. It is easy to read and write. One of the main reasons python was created was to address the observation "Code is read more than it is written". It's possible however to write terrible unreadable Python, and it is possible to write Python that is so advanced and uses many tricks that it is difficult to read, but it is very easy to make easily read Python

Fifth, you can make publication quality graphs with Matplotlib.

Sixth, you can access many powerful and fast functions used in science with Scipy.

Seventh, you can use python in notebooks much like Mathematica, it is awesome. They are called Jupyter Notebooks.

But python is an interpreted language, isn't it slower than a compiled language like c or Fortran??

Yes, this is true, but not if you use python wisely and as intended. Numpy is the heart of many python libraries and much of what you will be doing. When you create an array with Numpy it makes a contiguous sequence of data in RAM so it is quickly accessed. This is why you can't easily append things to Numpy Arrays because the next byte of data may be already occupied. When you tell Numpy to multiply things or sum them it does not do that with Python. It uses special hardware on your computer designed to do array math. Doing computations on hardware dedicated to do those computations is the fastest way to compute. This is how things like Apollo 11 worked even though computers were slow. It had dedicated hardware to do a small specific math or matrix operation very quickly (at the time).

Scipy on the other hand is often just wrappers for old Fortran code and thus is just as fast as that code. Many Scipy functions are decades old Fortran algorithms from publications.




What libraries and software should I have?
Numpy, Scipy, Matplotlib and Astropy will cover like 99\% of data analysis.

For software I recomend using Jupyter notebooks. For making big projects, or if you want real time code correction, I would use PyCharm. Jupyter Notebooks can do code correction, but PyCharm is better IMO. Downside is PyCharm is expert friendly. 

Always start with the latest python and then don't upgrade until you need to or are starting a new project on a new machine. You can break things by following upgrades sometimes even though they try to prevent that. There also usually isn't a good reason for most people. Make sure to get at least python3.0! 

To view images saved in the FITs file format, a common standard, download SAOImage. It is expert friendly, but veeeery powerful


