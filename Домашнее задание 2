using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace project2  {

public class Program
{
    public static void Main(string[] args)
    {
        var elementsCount = 0;

        while (elementsCount < 2)
        {
            try
            {
                Console.Write("Здравствуйте! Введите, пожалуйста, количество чисел из которых хотите найти второе наибольшее:\t ");
                elementsCount = int.Parse(Console.ReadLine());
                if (elementsCount < 2)
                {
                    Console.WriteLine("\nВведите минимум два числа для сравнения");
                }
            }

            catch (System.FormatException)
            {
                Console.WriteLine("\nКоличество должно быть целым числом");
            }

            
            finally { }
        }


        var myArray = new int[elementsCount];
        while (true)
        {
            try
            {
                for (int i = 0; i < myArray.Length; i++)
                {
                    Console.Write($"\nВведите любое положительное целое число{i}:\t ");
                    myArray[i] = int.Parse(Console.ReadLine());
                }


                int maxValue = int.MinValue;
                int secondMaxValue = int.MinValue;

                for (int i = 0; i < myArray.Length; i++)
                {
                    if (myArray[i] > maxValue)
                    {
                        secondMaxValue = maxValue;
                        maxValue = myArray[i];
                    }
                    else if (myArray[i] > secondMaxValue)
                    {
                        secondMaxValue = myArray[i];
                    }
                }

                Console.WriteLine($"\nВторое наибольшее число:{secondMaxValue} ");

                break;
            }

            catch (System.FormatException)
            {
                Console.WriteLine("\nУкажите целое число");
            }

        

            finally { }
        }
    }
}

}
