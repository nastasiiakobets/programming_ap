using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace array1
{
    class Program
    {
        static void Main(string[] args)
        {
          var array = CreateArray(2000,-1000,1000);

          Console.ReadLine();
        } 

         public static void Array1()
        {
          float[] a = new float[10];
          int k = 0;

          Console.WriteLine("enter your array a[10]");
          for(int i=0;i<10;i++)
          {
             a[i] = float.Parse( Console.ReadLine() );
             if (a[i]<0)
             {
              k++;
             }
          }
         Console.WriteLine(k+"- negative numbers");
         Console.WriteLine((10-k)+"- positive numbers");
         Console.ReadLine();
        }  
         static int[] CreateArray(int size, int min,int max)
        {
            int[] result = new int[size];
            var r = new Random();
            for(int i=0;i<size;i++)
            {
                result[i] = r.Next(min,max);
            }
            foreach(int item in result)
            {
                Console.WriteLine(item);
            }
            return result;
        }
         static void ArrayString(string value)
        {
            foreach(var item in value)
            {
                Console.WriteLine(item);
            }
                 Console.ReadLine();
        }
    }
}
