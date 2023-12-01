using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Simple Calculator");

        Console.Write("Enter first number: ");
        double num1 = Convert.ToDouble(Console.ReadLine());

        Console.Write("Enter second number: ");
        double num2 = Convert.ToDouble(Console.ReadLine());

        Console.WriteLine("\nChoose an operation:");
        Console.WriteLine("1. Addition (+)");
        Console.WriteLine("2. Subtraction (-)");
        Console.WriteLine("3. Multiplication (*)");
        Console.WriteLine("4. Division (/)");

        Console.Write("Enter the operation number: ");
        int choice = Convert.ToInt32(Console.ReadLine());

        double result = Calculator.PerformOperation(num1, num2, choice);

        Console.WriteLine($"Result: {result}");
    }
}
