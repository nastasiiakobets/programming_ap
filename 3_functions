sing System;
using System.Collections.Generic;
using System.Diagnostics.Metrics;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;


namespace kobets_1
{
    class Program
    {
        static void Main(string[] args)
        {
            float[] a = new float[10];


            Console.WriteLine("Menu : ");
            Console.WriteLine("1 - Add");
            Console.WriteLine("2 - Show");
            Console.WriteLine("3 - Search");
            Console.WriteLine("4 - Statistics");
            Console.WriteLine("5 - Exit");

            Console.WriteLine();
            Console.WriteLine("enter number: ");
            var n = Console.ReadLine();
            var w = false;

            while (w == false)
            {

                switch (n)
                {
                    case "1"://+
                        Add(a);
                        Console.ReadLine();
                        break;
                    case "2"://+
                        Show(a);
                        Console.ReadLine();
                        break;
                    case "3":
                        Search();
                        Console.ReadLine();
                        break;
                    case "4":
                        Statistics();
                        Console.ReadLine();
                        break;
                    case "5":
                        Exit();
                        return;
                        break;
                }
            }
            Console.ReadLine();
        }

        private static void Add(float [] a)
        {
            
            Console.WriteLine("enter your array a[10]");
            for (int i = 0; i < 10; i++)
            {
                a[i] = float.Parse(Console.ReadLine()); 
            }
 
        }
        static void Show(float[] a)
        {
            Console.WriteLine("your array: ");
            for (int i = 0; i < 10; i++)
            {
                Console.Write(a[i] +" ");
            }

        }
        static void Search()
        {

        }
        static void Statistics()

        {

        }
        static void Exit()
        {

            Program.Exit();

        }
    }
}
