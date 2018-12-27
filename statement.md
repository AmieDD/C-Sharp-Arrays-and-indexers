# C# [] Operator - Arrays and indexers

Code, Cosplay and Game - www.amiedd.com

```C# runnable

using System;

class PotionStrength 
{
   // Array of Potion Strength values
    private float[] potions = new float[10] { 56.2F, 56.7F, 56.5F, 56.9F, 58.8F, 
                                            61.3F, 65.9F, 62.1F, 59.2F, 57.5F };

    public int Length
    {
        get { return potions.Length; }
    }
    // Indexer declaration.
    // If index is out of range, the potions array will throw the exception.
    public float this[int index]
    {
        get
        {
            return potions[index];
        }

        set
        {
            potions[index] = value;
        }
    }
}

class MainClass
{
    static void Main()
    {
        PotionStrength potionStrength = new PotionStrength();
        // Use the indexer's set accessor
        potionStrength[3] = 58.3F;
        potionStrength[5] = 60.1F;

        // Use the indexer's get accessor
        for (int i = 0; i < 10; i++)
        {
            System.Console.WriteLine("Potion #{0} = {1}", i, potionStrength[i]);
        }

    }
}
/* Output:
        Potion #0 = 56.2
        Potion #1 = 56.7
        Potion #2 = 56.5
        Potion #3 = 58.3
        Potion #4 = 58.8
        Potion #5 = 60.1
        Potion #6 = 65.9
        Potion #7 = 62.1
        Potion #8 = 59.2
        Potion #9 = 57.5
    */

```

# C# [] Operator - Arrays and indexers

Square brackets ([]) are used for arrays, indexers, and attributes. They can also be used with pointers.
