1.A. using System;

namespace SumOfIntegers
{
    class Program
    {
        static void Main(string[] args)
        {
            // Prompt the user to enter two integers
            Console.WriteLine("Enter the first integer:");
            int num1 = Convert.ToInt32(Console.ReadLine());

            Console.WriteLine("Enter the second integer:");
            int num2 = Convert.ToInt32(Console.ReadLine());

            // Calculate the sum of the two integers
            int sum = num1 + num2;

            // Display the result
            Console.WriteLine("The sum of " + num1 + " and " + num2 + " is " + sum);

            Console.ReadLine();
        }
    }
}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------
1.B. using System;

namespace MaxIntegerValue
{
    class Program
    {
        static void Main(string[] args)
        {
            // Find the maximum value for integers
            int maxIntValue = int.MaxValue;

            // Assign the maximum value to two integer variables
            int num1 = maxIntValue;
            int num2 = maxIntValue;

            // Display the values of num1 and num2
            Console.WriteLine("num1: " + num1);
            Console.WriteLine("num2: " + num2);

            Console.ReadLine();
        }
    }
}

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------

2. using System;

class Program
{
    static void Main()
    {
      
        Console.Write("Enter Product ID: ");
        int productId = int.Parse(Console.ReadLine());

        Console.Write("Enter Product Name: ");
        string productName = Console.ReadLine();

        Console.Write("Enter Unit Price: ");
        decimal unitPrice = decimal.Parse(Console.ReadLine());

        Console.Write("Enter Quantity: ");
        int quantity = int.Parse(Console.ReadLine());

        decimal totalAmount = unitPrice * quantity;

       
        decimal discount = 0;

        if (totalAmount > 5000)
        {
            discount = 0.20m;
        }
        else if (totalAmount > 3000)
        {
            discount = 0.15m; 
        }
        else if (totalAmount > 1000)
        {
            discount = 0.10m; 
        }

        decimal discountAmount = totalAmount * discount;
        decimal finalAmount = totalAmount - discountAmount;

        Console.WriteLine("\nProduct Information:");
        Console.WriteLine($"Product ID: {productId}");
        Console.WriteLine($"Product Name: {productName}");
        Console.WriteLine($"Unit Price: {unitPrice:C}");
        Console.WriteLine($"Quantity: {quantity}");
        Console.WriteLine($"Total Amount: {totalAmount:C}");
        Console.WriteLine($"Discount Applied: {discount * 100}%");
        Console.WriteLine($"Discount Amount: {discountAmount:C}");
        Console.WriteLine($"Final Amount after Discount: {finalAmount:C}");
    }
}
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

3. using System;

class Program
{
    static void Main()
    {
        int patientId = 1;
        string patientName = "Raghu";
        int age = 45;
        string address = "Hyderabd, KPHB street 5";
        bool hasInsurance = true;
        double weightKg = 70.5;
        DateTime lastVisitDate = DateTime.Now.AddDays(-30);
        string diagnosis = "Hypertension";

        Console.WriteLine("Patient Details:");
        Console.WriteLine($"Patient ID: {patientId}");
        Console.WriteLine($"Patient Name: {patientName}");
        Console.WriteLine($"Age: {age}");
        Console.WriteLine($"Address: {address}");
        Console.WriteLine($"Has Insurance: {(hasInsurance ? "Yes" : "No")}");
        Console.WriteLine($"Weight: {weightKg} kg");
        Console.WriteLine($"Last Visit Date: {lastVisitDate.ToShortDateString()}");
        Console.WriteLine($"Diagnosis: {diagnosis}");
    }
}
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
