using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace practica01
{

    class Program
    {
        static void Main(string[] args)
        {
            int num1;
            int num2;
            int num3;
            int num4;
            int menor = 0;
            int mayor = 0;
            int suma = 0;
            int resta = 0;

            Console.WriteLine("ingrese el primer numero: ");
            num1 = int.Parse(Console.ReadLine());

            while (num1 <= 0)
            {
                Console.WriteLine("ingrese el primer numero: ");
                num1 = int.Parse(Console.ReadLine());

            }
            while (num1 >= 200)
            {
                Console.WriteLine("ingrese el primer numero: ");
                num1 = int.Parse(Console.ReadLine());
            }
  
            Console.WriteLine("ingrese el segundo numero: ");
            num2 = int.Parse(Console.ReadLine());
            while(num2 <= 0)
            {
                Console.WriteLine("ingrese el segundo numero: ");
                num2 = int.Parse(Console.ReadLine());

            }
            while(num2 == num1)
            {
                Console.WriteLine("ingrese el segundo numero: ");
                num2 = int.Parse(Console.ReadLine());
            }
            while (num2 >= 200)
            {
                Console.WriteLine("ingrese el segundo numero: ");
                num2 = int.Parse(Console.ReadLine());
            }
            
            Console.WriteLine("ingrese el tercer numero: ");
            num3 = int.Parse(Console.ReadLine());
            if (num3 <= 0)
            {
                Console.WriteLine("ingrese el tercer numero: ");
                num3 = int.Parse(Console.ReadLine());
            }
            while (num3 == num1)
            {
                Console.WriteLine("ingrese el tercer numero: ");
                num3 = int.Parse(Console.ReadLine());
            }
            while (num3 == num2)
            {
                Console.WriteLine("ingrese el tercer numero: ");
                num3 = int.Parse(Console.ReadLine());
            }
            while (num3 >= 200)
            {
                Console.WriteLine("ingrese el tercer numero: ");
                num3 = int.Parse(Console.ReadLine());
            }

            Console.WriteLine("ingrese el cuarto numero: ");
            num4 = int.Parse(Console.ReadLine());
            if (num4 <= 0)
            {
                Console.WriteLine("ingrese el cuarto numero: ");
                num4 = int.Parse(Console.ReadLine());
            }
            while (num4 == num1)
            {
                Console.WriteLine("ingrese el cuarto numero: ");
                num4 = int.Parse(Console.ReadLine());
            }
            while (num4 == num2)
            {
                Console.WriteLine("ingrese el cuarto numero: ");
                num4 = int.Parse(Console.ReadLine());
            }
            while (num4 == num3)
            {
                Console.WriteLine("ingrese el cuarto numero: ");
                num4 = int.Parse(Console.ReadLine());
            }
            while (num4 >= 200)
            {
                Console.WriteLine("ingrese el cuarto numero: ");
                num4 = int.Parse(Console.ReadLine());
            }

            if (num1 < num2 && num1 < num3 && num1 < num4)
            {
                menor = num1;
                Console.WriteLine("el numero menor es :" + num1);

            }
            else
            {
                if (num2 < num1 && num2 < num3 && num2 < num4)
                {
                    menor = num2;
                    Console.WriteLine("el numero menor es :" + num2);

                }
                else
                {
                    if (num3 < num1 && num3 < num2 && num3 < num4)
                    {
                        menor = num3;
                        Console.WriteLine("el numero menor es :" + num3);

                    }
                    else
                    {
                        menor = num4;
                        Console.WriteLine("el numero menor es : " + num4);
                    }
                }
            }
            if (num1 > num2 && num1 > num3 && num1 > num4)
            {
                mayor = num1;
                Console.WriteLine("el numero mayor es :" + num1);

            }
            else
            {
                if (num2 > num1 && num2 > num3 && num2 > num4)
                {
                    mayor = num2;
                    Console.WriteLine("el numero menomayor es :" + num2);

                }
                else
                {
                    if (num3 > num1 && num3 > num2 && num3 > num4)
                    {
                        mayor = num3;
                        Console.WriteLine("el numero mayor es :" + num3);

                    }
                    else
                    {
                        mayor = num4;
                        Console.WriteLine("el numero mayor es : " + num4);
                    }
                }
            }

            if (menor > 10)
            {
                suma = mayor + 10;
                Console.WriteLine("el numero mayor ahora es: " + suma);
            }
            if (mayor < 50)
            {
                resta = menor - 5;
                Console.WriteLine("el numero menor ahora  es: " + resta);
            }

            Console.ReadKey();
        }
        
    }
}
