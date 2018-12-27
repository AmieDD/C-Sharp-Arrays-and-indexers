# C# [] Operator - Arrays and indexers

Code, Cosplay and Game - www.amiedd.com

```C# runnable

using System;

class Operators 
{
    static void Main() 
    {
    fib[0] = fib[1] = 1;
    for (int i = 2; i < 100; ++i) fib[i] = fib[i - 1] + fib[i - 2];
    
     Console.WriteLine(fib);   
    }
    
   
}

```

# C# [] Operator - Arrays and indexers

Square brackets ([]) are used for arrays, indexers, and attributes. They can also be used with pointers.
