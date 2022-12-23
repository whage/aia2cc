### Links to the pdf documents:
- https://github.com/namin/inc
	- Link to the short paper: https://github.com/namin/inc/blob/master/docs/paper.pdf
	- Link to the mentioned full tutorial: https://github.com/namin/inc/blob/master/docs/tutorial.pdf
- https://github.com/carld/compiler-tutorial
	- Link to the short paper: https://github.com/carld/compiler-tutorial/blob/master/11-ghuloum.pdf
	- Link to the mentioned full tutorial: https://github.com/carld/compiler-tutorial/blob/master/compilers-tutorial-2006-09-16.pdf

### --omit-frame-pointer
https://people.cs.rutgers.edu/~pxk/419/notes/frames.html#:~:text=A%20frame%20pointer%20(the%20ebp,offsets%20to%20the%20frame%20pointer.

> Each function has local memory associated with it to hold incoming parameters, local variables, and (in some cases) temporary variables. This region of memory is called a stack frame and is allocated on the process’ stack. A frame pointer (the ebp register on intel x86 architectures, rbp on 64-bit architectures) contains the base address of the function’s frame. The code to access local variables within a function is generated in terms of offsets to the frame pointer. The stack pointer (the esp register on intel x86 architectures or rsp on 64-bit architectures) may change during the execution of a function as values are pushed or popped off the stack (such as pushing parameters in preparation to calling another function). The frame pointer doesn’t change throughout the function.

https://stackoverflow.com/questions/14666665/trying-to-understand-gcc-option-fomit-frame-pointer

> It's really about how well the compiler manages to track how the stack is used, and where things are on the stack (local variables, arguments passed to the current function and arguments being prepared for a function about to be called)