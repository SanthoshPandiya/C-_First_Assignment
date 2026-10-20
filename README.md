using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace DotNet_assignment1
{
    internal class Program
    {
        static void Main(string[] args)
        {

          
                Console.WriteLine("=== 1. OPERATORS DEMO ===");
                int a = 10;
                int b = 3;

                // Arithmetic
                Console.WriteLine($"a + b = {a + b}"); // 13
                Console.WriteLine($"a % b = {a % b}"); // 1 (Remainder)

                // Relational & Logical
                bool isValid = (a > b) && (b > 0);
                Console.WriteLine($"Is valid (a > b and b > 0)? {isValid}"); // True


                Console.WriteLine("\n=== 2. TYPE CASTING DEMO ===");

                // Implicit Casting (small to large)
                int myInt = 9;
                double myDouble = myInt;
                Console.WriteLine($"Implicit cast (int to double): {myDouble}"); // Output: 9

                // Explicit Casting (large to small)
                double myPreciseDouble = 9.87;
                int myConvertedInt = (int)myPreciseDouble;
                Console.WriteLine($"Explicit cast (double to int): {myConvertedInt}"); // Output: 9 (decimal dropped)


                Console.WriteLine("\n=== 3. LOOPING CONDITIONS DEMO ===");

                // A. For Loop
                Console.WriteLine("--- For Loop ---");
                for (int i = 1; i <= 3; i++)
                {
                    Console.WriteLine($"For loop iteration: {i}");
                }

                // B. While Loop
                Console.WriteLine("\n--- While Loop ---");
                int count = 1;
                while (count <= 2)
                {
                    Console.WriteLine($"While loop count: {count}");
                    count++;
                }

                // C. Foreach Loop (Arrays)
                Console.WriteLine("\n--- Foreach Loop ---");
                string[] subjects = { "Math", "Science", "C# Programming" };
                foreach (string subject in subjects)
                {
                    Console.WriteLine($"Subject: {subject}");
                }
            }
        }
    }
    

