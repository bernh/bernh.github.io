+++
title = "Old habbits - good habbits?"
date = 2023-11-20
+++

While learning multiple programming languages in the past, C was the first language
that I used professionally. While reading chapter 1.1 I noticed a personal habbit 
that originates from these times. Or should I say from the deficencies of this language?
C differentiates between declaration and definition and requires declaration before usage. 
Without going into the details what this exactly means, it bascially boils down to this 
typical structure:

```C
int helper_function(int param) {
  // ... do something and return
}

int main (int argc, char **argv) {
  // ... whatever
  x = helper_function(y);
  // ... continue
}
```

The `helper_function` needs to be *above* the `main` function otherwise the 
compiler will complain. ([^1]: Yes, I know, technically only the declaration needs to be above
but this is the way I ended up writing 99% of my C code.) Whenever a new function needs to
be introduced, go up and insert above. 

And I realized that I'm doing this also in my Python ([^2]: In Python there is of course this 
weird `if __name__ == "__main__"` thing but I always call `main()` there and this function can be on the top) and Rust code while it's not necessary
there. This observation sent me down a rabbit hole of stack overflow questions and tons of
advice for different programming languages. Anyway, I have made a decision: I will write code
top-to-bottom in the future.

