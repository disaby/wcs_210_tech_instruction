# WCS 210 Tech Instruction Group 4

## How to debug C++ code in Visual Studio

### Introduction:

Welcome to this technical instruction on how to compile C++ code in VS Code! A compiler is responsible for translating text written in a programming language into machine codes. In this instruction, we will guide you through the step-by-step process of installing a compiler on your computer. This instruction is designed for Computer Science students who may not have prior experience with VS Code. The reason for this is the use of Ubuntu as a code editor.

We will use clear and concise language and provide visual aids to help you easily follow along. By the end of this instruction, you will be able to successfully compile C++ code in VS Code and begin writing your code in a more convenient program.


### Prerequisites:
  
1. A C++ compiler: Before you can start debugging your C++ code, you need to have a compiler installed on your computer. There are many options available for C++ compilers, such as GCC, Clang, and Visual C++. You should choose a compiler that is compatible with the debugger you plan to use.
2. You will need a program that allows you to write and edit C++ code. In our case it is a full-featured IDE like Visual Studio Code. You should know how to do basic things in VS Code (open folder, create new file).
3. A basic understanding of C++ programming: In order to effectively debug your C++ code, you should have a basic understanding of C++ programming concepts and syntax.

  
### Definitions:
  
1. C++: a general-purpose programming language that supports object-oriented programming and is commonly used for developing system software, applications, and video games.
2. Compiler: a computer program that translates source code written in a high-level programming language into machine code that can be executed by a computer.

### Step by step guide:

#### 1. Install the C++ extension:
Open Visual Studio Code and click on the "Extensions" icon on the left-hand side of the window. In the search bar, type "C++" and select the "C++" extension from the list. Click the "Install" button to install the extension.

<p align="center">
  <img src="https://user-images.githubusercontent.com/123377628/219964667-f0b4743d-4a82-484d-9dba-0dbeeca23049.jpeg" height=300>
</p>


#### 2. Install a C++ compiler:
Visual Studio Code does not come with a built-in C++ compiler, so you will need to download and install one separately. One option is to download the MinGW compiler from this [website](https://sourceforge.net/projects/mingw/). Follow the installation prompts to install the compiler on your computer.

<p align="center">
  <img src="https://user-images.githubusercontent.com/123377628/219964710-a16bc2d2-8cfb-46ff-bc3c-d4e50cc92d88.jpeg" height=300>
</p>

#### 3. Add MinGW to the PATH environment variable: 
To use the MinGW compiler in Visual Studio Code, you will need to add it to the PATH environment variable. Right-click on the "Computer" or "This PC" icon on your desktop and select "Properties". This will open the System window.

#### 4. Click on "Advanced system settings" on the left-hand side of the window. 
This will open the System Properties window. Click on the "Environment Variables" button at the bottom of the window. This will open the Environment Variables window.


<p align="center">
  <img src="https://user-images.githubusercontent.com/123377628/219964745-c452e57a-56a6-4264-a683-c7274655c105.jpeg" height=300>
</p>


    
#### 5. Under "System variables", scroll down and find the "Path" variable. 
Select it and click on "Edit". In the "Edit Environment Variable" window, click on "New" and type the path to the MinGW bin directory, using a backslash to separate it from other paths in the list. For example, if MinGW is installed in the default directory, the path to the bin directory would be “C:\MinGW\bin”.

<p align="center">
  <img src="https://user-images.githubusercontent.com/123377628/219964777-b8404348-4134-4a10-a9e7-d679cad8faa6.jpeg" height=300>
</p>
    
#### 6. Click "OK" to close all the windows. 
Now your Visual Studio Code is ready to compile C++ code.


### Let’s do a little check
#### Configure Visual Studio Code: 
Open Visual Studio Code and create a new folder where you will store your C++ projects. Then, create a new file in the folder with a .cpp file extension (for example, hello.cpp). In the top menu bar, click on "Terminal" and select "New Terminal" to open a new terminal window in Visual Studio Code.

<p align="center">
  <img src="https://user-images.githubusercontent.com/123377628/219964808-85f1f7a4-75a1-44e1-9754-1b885f121258.jpeg" height=300>
</p>

  
#### Compile and run your C++ code:
In the terminal window, navigate to the folder where you saved your .cpp file using the cd command. Then, use the g++ command to compile your code (for example, g++ hello.cpp -o output). Once the compilation is complete, you can run the compiled program by typing “./output” in the terminal window.

> Code to compile:
```
#include <iostream>

int main() 
{
  std::cout<<"Hello world!";
  return 0;
}
```

> Code to print result:
```
g++ hello.cpp -o output
./output
```


### Troubleshooting:

The first problem you may encounter is the error “The file has been downloaded incorrectly!”

It is very likely that you did not use the download link in these instructions and downloaded the installer from the official website. The problem is that the official installer has been broken for years. 

To solve this problem, use the link provided in the instructions.

<p align="center">
  <img src="https://user-images.githubusercontent.com/123377628/221936742-023458cc-38a6-4449-be1d-448600c5d097.jpeg" height=300>
</p>
Another problem concerns owners of the new Windows 11. After the latest update, the "This PC" icon disappears from the desktop.

To get the icon back, press Win + E. This will open the explorer. Drag and drop "This PC" onto the desktop. This will bring the icon back.

<p align="center">
  <img src="https://user-images.githubusercontent.com/123377628/221936786-bca47800-d08f-4597-913c-37cc53ecaead.jpeg" height=300>
</p>


### Conclusion
Compiling C++ code in Visual Studio is a fundamental process for any developer who wants to build complex applications. Through this guide, we have explored how to set up Visual Studio for C++ development, create a C++ project, add source code files to the project, and compile the code. We've also covered how to handle common errors that may arise during the compilation process.
