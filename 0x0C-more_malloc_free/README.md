
0x0C. C - More malloc, free
C
Memory allocation
 By: Julien Barbier
 Weight: 1
 Project will start Oct 6, 2022 6:00 AM, must end by Oct 7, 2022 6:00 AM
 was released at Oct 6, 2022 12:00 PM
 An auto review will be launched at the deadline
Concepts
For this project, we expect you to look at this concept:

Automatic and dynamic allocation, malloc and free
Resources
Read or watch:

Do I cast the result of malloc?
man or help:

exit (3)
calloc
realloc
Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

General
How to use the exit function
What are the functions calloc and realloc from the standard library and how to use them
Copyright - Plagiarism
You are tasked to come up with solutions for the tasks below yourself to meet with the above learning objectives.
You will not be able to meet the objectives of this or any following project by copying and pasting someone else’s work.
You are not allowed to publish any content of this project.
Any form of plagiarism is strictly forbidden and will result in removal from the program.
Requirements
General
Allowed editors: vi, vim, emacs
All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
All your files should end with a new line
A README.md file, at the root of the folder of the project is mandatory
Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
You are not allowed to use global variables
No more than 5 functions per file
The only C standard library functions allowed are malloc, free and exit. Any use of functions like printf, puts, calloc, realloc etc… is forbidden
You are allowed to use _putchar
You don’t have to push _putchar.c, we will use our file. If you do it won’t be taken into account
In the following examples, the main.c files are shown as examples. You can use them to test your functions, but you don’t have to push them to your repo (if you do we won’t take them into account). We will use our own main.c files at compilation. Our main.c files might be different from the one shown in the examples
The prototypes of all your functions and the prototype of the function _putchar should be included in your header file called main.h
Don’t forget to push your header file
Quiz questions
Question #0
To allocate enough space for an array of 10 integers (on a 64bit, Linux machine), I can use:


malloc(64 * 10)


malloc(10 * int)


malloc(10 * sizeof(int))

Question #1
If I want to copy the string “Best School” into a new space in memory, I can use this statement to reserve enough space for it (select all valid answers):


malloc(sizeof(“Best School”))


malloc(strlen(“Best School”))


malloc(11)


malloc(12)


malloc(sizeof(“Best School”) + 1)


malloc(strlen(“Best School”) + 1)

Question #2
malloc returns a pointer


True


False

Question #3
malloc returns an address


True


False

Question #4
What is wrong with this code:



int cp(void)
{
    char *s;

    s = malloc(12);
    strcpy(s, "Best School");
    return (0);
}

You don’t have enough space to store the copy of the string “Best School”


There is no comment


You can’t call strcpy with a string literal


malloc can fail so we should check its return value all the time before using the pointers returned by the function.

Question #5
You can do this:

free("Best School");

Yes


No

Question #6
You can do this:

char str[] = "Best School";

free (str);

Yes


No

Question #7
You can do this:

char *s;

s = strdup("Best School");
if (s != NULL)
{
    free(s);
}

Yes


No

Question #8
The memory space reserved when calling malloc is on:


The stack


The heap

Question #9
What will you see on the terminal?

int main(void)
{
    int *ptr;

    *ptr = 98;
    printf("%d\n", *ptr);
    return (0);
}

0


98


It doesn’t compile


Segmentation Fault

Please make sure to validate all quiz questions before moving on to project tasks
Copyright © 2022 ALX, All rights reserved.
