# cpp command
cpp is the C language preprocessor, it is automatically used by your C compiler to transform your program before compilation. It is also termed as a macro processor because it is used to give abbreviations for the longer piece of code. It can only be used with C, C++ and Objective-C source code. Using with other programming languages may cause uncertain problems. Syntax:

Some Important Options:
-D name : Predefine name as a macro.
-D name=definition : The contents of definition are tokenized and processed as if they are written in program itself.
-U name : Cancel any previous definition of macro.
-undef : Do not predefine any system-specific or GCC-specific macros. The standard predefined macros remain defined.
-I dir : Add the directory dir to the list of directories to be searched for header files.
-Wall : Turns on all optional warnings which are desirable for normal code.
-Wcomments : Warn whenever a comment-start sequence /* appears in a /* comment, or whenever a backslash-newline appears in a // comment.
-Wendif-labels : Warn whenever an #else or an #endif are followed by text.
-w : Suppress all warnings, including those which GNU CPP issues by default.
-M : Instead of outputting the result of preprocessing, output a rule suitable for make describing the dependencies of the main source file.
-MM : Like -M but do not mention header files that are found in system header directories.
-x c
-x c++
-x objective-c
-x assembler-with-cpp : All four above Specify the source language: C, C++, Objective-C, or assembly. This has nothing to do with standards conformance or extensions; it merely selects which base syntax to expect.

## references
1. <https://www.geeksforgeeks.org/cpp-command-in-linux-with-examples/>