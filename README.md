using System;

 Partiendo del ejercicio anterior, determinar el literal según la calificación obtenida del estudiante:
//  Calificación Situación
//  90 – 100 Excelente
//  80 – 89 Muy bueno
//  75 – 79 Bueno
//  70 – 74 Regular
//  Menos de 70 deficiente

namespace PromedioNotas
{
    class Program
    {
        static void Main(string[] args)
        {
            double N1, N2, N3, N4, promedio;

            Console.WriteLine(" ~ Ingrese la primera nota:");
            N1 = double.Parse(Console.ReadLine());

            Console.WriteLine(" ~ Ingrese la segunda nota:");
            N2 = double.Parse(Console.ReadLine());

            Console.WriteLine(" ~ Ingrese la tercera nota:");
            N3 = double.Parse(Console.ReadLine());

            Console.WriteLine(" ~ Ingrese la cuarta nota:");
            N4 = double.Parse(Console.ReadLine());

            promedio = (N1 + N2 + N3 + N4) / 4;

            Console.WriteLine($" ~ El promedio es: {promedio}");


            Console.Write(" ~ Nota obtenida: ");
            if (promedio >= 90 && promedio <= 100)
            {
                Console.WriteLine("Excelente");
            }
            else if (promedio >= 80 && promedio <= 89)
            {
                Console.WriteLine("Muy bueno");
            }
            else if (promedio >= 75 && promedio <= 79)
            {
                Console.WriteLine("Bueno");
            }
            else if (promedio >= 70 && promedio <= 74)
            {
                Console.WriteLine("Regular");
            }
            else
            {
                Console.WriteLine("Deficiente");
            }
        }
    }
}
