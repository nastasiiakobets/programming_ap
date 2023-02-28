using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp144
{
    class Program
    {
        static void Main(string[] args)
        {

            var input = "Radar";
            var result = IsPaindrome(input);
            Console.ReadLine();
        }  
        private static void PrintTreangle(int value)
        {//*******2.2*******
            for (int i = 1; i <= value; i++)
            {
                Console.WriteLine(new string('*', i));
            }
        }
        private static void PrintNum(int value)
        { //*******2.1*******

            Console.WriteLine("from: ");
            var a1 = Console.ReadLine();
            int a = Convert.ToInt32(a1);

            Console.WriteLine("to: ");
            var b1 = Console.ReadLine();
            int b = Convert.ToInt32(b1);

            for (int f = a; f <= b; f++)
            {
                int n = 0;
                for (int i = 2; i < f; i++)
                {
                    if (f % i == 0)
                    {
                        n = 1;
                    }
                }
                if (n == 0)
                {
                    Console.Write(f + " ");
                }
            }
        }
        private static void PrintI()
        {
           // *******1.1*******
            var w = false;

            while (w == false)
            {
                Console.Clear();
                Console.WriteLine("MENU:");
                Console.WriteLine("1 - a");
                Console.WriteLine("2 - b");
                Console.WriteLine("3 - c");
                Console.WriteLine("4 - d");
                Console.WriteLine("5 - exit");
                Console.WriteLine("");
                Console.WriteLine("enter:   ");
                var enter = Console.ReadLine();

                switch (enter)
                {
                    case "1":
                        Console.WriteLine("option a: ");
                        Console.WriteLine("a = ");
                        var a = Console.ReadLine();
                        Console.WriteLine("b = ");
                        var b = Console.ReadLine();
                        Console.WriteLine("c = ");
                        var c = Console.ReadLine();

                        int a1 = Convert.ToInt32(a);
                        int b1 = Convert.ToInt32(b);
                        int c1 = Convert.ToInt32(c);

                        if ((a1 * a1 + b1 * b1) == c1 * c1)
                        {
                            Console.WriteLine("tak");
                        }
                        else
                        {
                            Console.WriteLine("nie");
                        }
                        Console.ReadLine();
                        break;

                    case "2":

                        break;
                    case "3":
                        Console.WriteLine("option c: ");
                        break;
                    case "4":
                        Console.WriteLine("option d: ");
                        break;
                    case "5":
                        Console.WriteLine("exit");
                        Console.WriteLine("yes or no?");
                        var answer = Console.ReadLine();
                        if (answer == "yes")
                        {
                            return;
                        }
                        break;
                }
            }

            Console.ReadLine();
        }
        public static bool IsPaindrome(string text)
        {
            text = text.ToUpper();
            int j = text.Length - 1;

            for(int i = 0; i < j; i++)
            {
                if (text[i] != text[j])
                {
                    return false;
                }
                j--;
            }
            return true;
        }

    }
}
