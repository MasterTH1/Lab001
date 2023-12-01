using System;

class Calculator
{
    public static double PerformOperation(double num1, double num2, int choice)
    {
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
                    Environment.Exit(0);
                }
                break;
            default:
                Console.WriteLine("Invalid choice.");
                Environment.Exit(0);
                break;
        }

        return result;
    }
}
