**SAILOR'S CODING STANDARDS**

## 1.  **Introduction**

   This document servers as the definition of Sailor’s general coding standards
   for source code in the different kinds of programming languages.

## 2.  **Source file basics**

### &nbsp; 2.1.  **File name**  
&nbsp;&nbsp;&nbsp;&nbsp;Every file must be named following those rules:

-   Every file must be written in “CamelCase”.

    -   Examples:

>   &nbsp;&nbsp;&nbsp;&nbsp;FileName, Test01, TestFileOfFunction

-   Every filename must be significant.

    -   Examples:

>   &nbsp;&nbsp;&nbsp;&nbsp;FeatureX, HomePage

-   Filenames can’t start with numbers.

### &nbsp;2.2.  **Source file structure**  
&nbsp;&nbsp;&nbsp;&nbsp;A source file consists of, in order:  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- License or copyright information, if present  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Package statement  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Import statements  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Exactly one top-level class  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;- Exactly one blank line separates each section that is present.

## 3.  **Code Formatting**

### &nbsp; 3.1.  **Braces**

#### &nbsp;&nbsp;&nbsp; 3.1.1.  **Braces use**   
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Braces are used with every statement, when they programming language is structured to do so.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Braces must be used even if the body is empty or contains only a single line.

#### &nbsp;&nbsp;&nbsp; 3.1.2.  **Braces style**  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Braces must follow the “Egyptian brackets” style or Kernighan and Ritchie style.

-   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Examples:

>   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;if (a == b) {  
>   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;printf("hello");  
>   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;}

### &nbsp; 3.2.  **Horizontal alignment**

&nbsp;&nbsp;&nbsp;&nbsp;Terminology Note: Horizontal alignment is the practice of aligning certain part of the code with the following lines.
&nbsp;&nbsp;&nbsp;&nbsp;Horizontal alignment is not required, even if is permitted.

-   &nbsp;&nbsp;&nbsp;&nbsp;Examples:

>   &nbsp;&nbsp;&nbsp;&nbsp;int a = 0; //not aligned  
>   &nbsp;&nbsp;&nbsp;&nbsp;int b = 0; //not aligned

### &nbsp; 3.3.   **Spacing between lines**

&nbsp;&nbsp;&nbsp;&nbsp;When the programming language permit it, the programmer must put empty lines in this cases:
-   &nbsp;&nbsp;&nbsp;&nbsp;2 empty lines between methods.
-   &nbsp;&nbsp;&nbsp;&nbsp;1 empty line between logically different blocks.
    -   &nbsp;&nbsp;&nbsp;&nbsp;Examples:

>   &nbsp;&nbsp;&nbsp;&nbsp;int a = 0;  
>   &nbsp;&nbsp;&nbsp;&nbsp;int b = 0;  
>
>   &nbsp;&nbsp;&nbsp;&nbsp;methodA(){  
>   &nbsp;&nbsp;&nbsp;&nbsp;print(something);  
>   &nbsp;&nbsp;&nbsp;&nbsp;}
>  
>   &nbsp;&nbsp;&nbsp;&nbsp;methodB(){  
>   &nbsp;&nbsp;&nbsp;&nbsp;print(methodA());  
>     
>   &nbsp;&nbsp;&nbsp;&nbsp;print(somethingDifferent);  
>   &nbsp;&nbsp;&nbsp;&nbsp;}

## 4.  **Declarations**

### &nbsp; 4.1.  **Variables**  
&nbsp;&nbsp;&nbsp;&nbsp;Variables must be declared in “lowerCamelCase” and the name must be
&nbsp;&nbsp;&nbsp;&nbsp;significant.

### &nbsp; 4.2.  **Methods and classes**  
&nbsp;&nbsp;&nbsp;&nbsp;Methods and classes must be declared in “CamelCase” and the name must be
&nbsp;&nbsp;&nbsp;&nbsp;significant.
