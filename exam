using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace zad1
{
    static class Program
    {
        static void Main(string[] args)
        {

            var w = false;
            while (w == false)
            {
                Console.Clear();
                Console.WriteLine("MENU:");
                Console.WriteLine("1 - sortowanie liczb");
                Console.WriteLine("2 - sprawdza adres e-mail");
                Console.WriteLine("3 - rysowania prostokąta");
                Console.WriteLine("4 - exit");
                Console.WriteLine("");
                Console.WriteLine("enter:   ");
                var enter = Console.ReadLine();

                switch (enter)
                {

                    //sortowania liczb
                    case "1":
                        Console.WriteLine("--------Sortowanie w porządku rosnącym---------");
                        var t = false;
                        while (t==false) {
                            Console.Write("enter 3 element: ");
                            var parts = Console.ReadLine().Split(new[] { " " }, StringSplitOptions.RemoveEmptyEntries);
                            if (parts.Length >= 3)
                            {
                                var array = new int[parts.Length];
                                for (int i = 0; i < parts.Length; i++)
                                {
                                    array[i] = Convert.ToInt32(parts[i]);
                                }

                                Console.WriteLine("new array: {0}", string.Join(", ", Sortowanie(array)));
                                t = true;
                            }
                            else
                                Console.WriteLine("error and enter again");
                            Console.ReadLine();
                        }
                        break;

                        //sprawdza adres e-mail
                    case "2":
                        Console.WriteLine("--------Sprawdza adres e-mail---------");
                        Console.WriteLine("enter e-mail:");
                        var e = Console.ReadLine();

                        Email(e);
                        Console.ReadLine();
                        break;

                        //rysowanie prostokąta
                    case "3":
                        Console.WriteLine("--------Rysowania prostokąta---------");
                        var d = false;
                        while (d == false)
                        {
                            try
                            {
                                Console.Write("Podaj długość: ");
                                var a = Console.ReadLine();
                                int a1 = Convert.ToInt32(a);
                                Console.Write("Podaj szerokość: ");
                                var b = Console.ReadLine();
                                int b1 = Convert.ToInt32(b);
                                Console.Write("Podaj znak: ");
                                var c = Console.ReadLine();
                                char c1 = Convert.ToChar(c);

                                Rysowanie(a1, b1, c1);
                                d = true;
                            }
                            catch(System.FormatException)
                            {
                                Console.WriteLine("error and enter again");
                            }

                        }
                        Console.ReadLine();
                        break;

                        //exit
                    case "4":
                        Console.WriteLine("-----exit-----");
                        Console.WriteLine("yes or no?");
                        var answer = Console.ReadLine();
                        if (answer == "yes")
                        {
                            return;
                        }
                        break;
                   default:
                        Console.WriteLine("error and enter again");
                        Console.ReadLine();
                        break;
                }
            }

            Console.ReadLine();
        }

        //1
        static int[] Sortowanie(int[] array)
        {

                var len = array.Length;
                for (var i = 1; i < len; i++)
                {
                    for (var j = 0; j < len - i; j++)
                    {
                        if (array[j] > array[j + 1])
                        {
                            Swap(ref array[j], ref array[j + 1]);
                        }
                    }
                }

                return array;

        }
        static void Swap(ref int e1, ref int e2)
        {
            var temp = e1;
            e1 = e2;
            e2 = temp;
        }

        //2
        static void Email(string email)
        {
            if (!IsValid(email))
            {
                Console.WriteLine("error (wrong email adress)");
                return;
            }

            string[] parts = email.Split('@');
            string username = parts[0];
            string domain = parts[1];

            username = username.ToUpper();
            domain = domain.ToUpper();

            Console.WriteLine("nazwa użytkownika " + username + " domena: " + domain);
        }
        public static bool IsValid(string email)
        {
            var num = 0;
            foreach (char c in email)
            {
                if (c == '@')
                {
                    num++;
                }
            }

            if (num != 1)
            {   Console.Write("liczba znaków '@'= "+num);
                return false;
            }
            string[] parts = email.Split('@');
            if (parts[0] == "" || parts[1] == "" || email.Contains(" "))
            {
                return false;
            }
            return true;
        }

        //3
        private static void Rysowanie(int a, int b, char znak)
        {
            Console.WriteLine();
                for (int i = 1; i <= b; i++)
                {
                    Console.WriteLine(new string(znak, a));
                }
        }
    }
}
