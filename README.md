# interfaces in C#

# c# interfaces are a contract between methods to use a set of methods.

## interface

```cs
public interface IAnimal
{
    void move()
}
```

## Class inheriting

```cs
public class Cat: IAnimal
{
    void move()
    {
        System.Console.WriteLine("the cat moves");
    }
}
```

## Declaring new class

```cs
class Program
{
    static void Main(string[] args)
    {
        IAnimal cat1 = new Cat();
        cat1.move();
    }
}
```

===

## this will throw an error for not implementing void move()

```cs
public class Dog: IAnimal
{

}
```

===
