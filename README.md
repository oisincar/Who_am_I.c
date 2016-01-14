#Who am I.c
I'm not sure if this really belongs here, but it sucks to spend a long time on something only to leave it in some random folder so.. Here it is anyway. My first (intentional, at least) attempt at obfuscated c code.

It prints "Oisin" followed by a newline, but the letters making up my second name; Carroll, are the only ones in the source code.
``` C
#include "stdio.h"
main(_){return!((-~_<<_/_<<_/_)/
  ' ')?main(-~_),printf(
    "%C",((_*((_*
      'a'*(_-
        'r'/6)+(1110*
          'r'<<_/_)/19)*_-7*(
            'o'>>_/_)*18*'!'/5)+(
              'L'<<10))*(_<<_/_)-(415*
                'l'<<4)/9+_*(_*_*_-3221*
                  '.'/23+_))/('<'<<_/_)):0;}
 ```

You're welcome to figure out how it works yourself, or you can read the comment within my attempt at spoiler tag below.

 <details> 
  <summary>**Click here for an explanation.**</summary>
   *  The characters come from a 6th order polynomial equation, the function prints one letter per recursion, increasing the value subbed in each time. I used an on-line maths engine (not wolfram-alpha, I can't remember what it was atm.) to generate it from some a series of simple ```a + bx + cx^2 + dx^3 +....= assci value``` equasions.

   *  ```((-~_<<_/_<<_/_)/' ')?``` on the first line means: ```if((x+1)*4/32)``` which is equilanent to ```if(x<7)```. This stops the looping.
   
   *  ```_``` is actually a variable name, and is the only variable in the program. It's declared as an int with the value of 1 in the main function header. It throws a warning, but it works.

   *  ```-~x``` is the same as ```x+1```. (Because of two's complement.. or something? I just stole it from somewhere.)
</details>

