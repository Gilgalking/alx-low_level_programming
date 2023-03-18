malloc returns a void pointer (void *), which can be cast to any other pointer type.
If malloc cannot allocate the requested amount of memory, it returns a null pointer (NULL).
The amount of memory allocated by malloc may be larger than the amount requested, due to internal memory alignment requirements.
It is important to call free on each pointer returned by malloc, otherwise the program may leak memory.
Calling free on a null pointer has no effect.
