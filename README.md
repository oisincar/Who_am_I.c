#Who am I.c
I'm not sure if this really belongs here, but it sucks to spend a long time on something only to leave it in some random folder so.. Here it is anyway. My first (intentional, anyway) attempt at obfuscated c code.

It prints "Oisin\n", with my second name; Carroll, in the source code. 

You're welcome to figure out how it works yourself, or you can read the comment within that attempt at spoiler tag below.

 <details> 
  <summary>Click here for an explanation.</summary>
   *  The characters come from a 6th order polynomial equation, the function prints one letter per recursion, increasing the value subbed in each time. I used an on-line maths engine (not wolfram-alpha, I can't remember what it was atm.) to generate it from some a series of simple ```a + bx + cx^2 + dx^3 +....= assci value``` equasions.

   *  ```((-~_<<_/_<<_/_)/' ')?``` on the first line means: ```if((x+1)*4/32)``` which is equilanent to ```if(x!=7)```. This stops the looping.
   
   *  ```_``` is actually a variable name, and is the only variable in the program. It's declared as an int in the main function header since that's the default. It throws a warning, but it works.

   *  ```-~x``` is the same as ```x+1```. (Because of two's complement.. or something? I just stole it from somewhere.)
</details>

