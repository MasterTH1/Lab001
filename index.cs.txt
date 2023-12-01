using System;

class Calculator
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

        double result = 0;

        switch (choice)
        {
            case 1:
                result = num1 + num2;
                break;
            case 2:
                result = num1 - num2;
                break;
            case 3:
                result = num1 * num2;
                break;
            case 4:
                if (num2 != 0)
                {
                    result = num1 / num2;
                }
                else
                {
                    Console.WriteLine("Cannot divide by zero.");
                    return;
                }
                break;
            default:
                Console.WriteLine("Invalid choice.");
                return;
        }

        Console.WriteLine($"Result: {result}");
    }
}
