using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Hotel_Room
{
    class Program
    {
        static void Main(string[] args)
        {
            string month = Console.ReadLine().ToLower();
            int night = int.Parse(Console.ReadLine());

            if (month == "may" || month == "october")
            {
                if (night > 14)
                {
                    double studioPrice = 50 - (50 * 0.3);
                    double apartmentPrice = 65 - (65 * 0.1);
                    Console.WriteLine("Apartment: {0:f2} lv.", night * apartmentPrice);
                    Console.WriteLine("Studio: {0:f2} lv.", night * studioPrice);
                }
                else if (night > 7 && night <= 14)
                {
                    double studioPrice = 50 - (50 * 0.05);
                    double apartmentPrice = 65;
                    Console.WriteLine("Apartment: {0:f2} lv.", night * apartmentPrice);
                    Console.WriteLine("Studio: {0:f2} lv.", night * studioPrice);
                }
                else
                {
                    double studioPrice = 50;
                    double apartmentPrice = 65;
                    Console.WriteLine("Apartment: {0:f2} lv.", night * apartmentPrice);
                    Console.WriteLine("Studio: {0:f2} lv.", night * studioPrice);
                }

            }
            else if (month == "june" || month == "september")
            {
                if (night > 14)
                {
                    double studioPrice = 75.20 - (75.20 * 0.2);
                    double apartmentPrice = 68.70 - (68.70 * 0.1);
                    Console.WriteLine("Apartment: {0:f2} lv.", night * apartmentPrice);
                    Console.WriteLine("Studio: {0:f2} lv.", night * studioPrice);
                }

                else
                {
                    double studioPrice = 75.20;
                    double apartmentPrice = 68.70;
                    Console.WriteLine("Apartment: {0:f2} lv.", night * apartmentPrice);
                    Console.WriteLine("Studio: {0:f2} lv.", night * studioPrice);
                }
            }
            else if (month == "july" || month == "august")
            {
                if (night > 14)
                {
                    double studioPrice = 76;
                    double apartmentPrice = 77 - (77 * 0.1);
                    Console.WriteLine("Apartment: {0:f2} lv.", night * apartmentPrice);
                    Console.WriteLine("Studio: {0:f2} lv.", night * studioPrice);
                }

                else
                {
                    double studioPrice = 76;
                    double apartmentPrice = 77;
                    Console.WriteLine("Apartment: {0:f2} lv.", night * apartmentPrice);
                    Console.WriteLine("Studio: {0:f2} lv.", night * studioPrice);
                }
            }
        }
    }
}
