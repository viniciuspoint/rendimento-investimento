using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace tabela_6_meses_part2
{
    internal class Program
    {
        static void Main(string[] args)
        {
            double mon_inicial = 3.800;
            double juros_mes = 1.25 / 100;
            int seis_meses = 6;
         
            Console.WriteLine("mes\tdinheiro");
            for (int mes = 1; mes <= seis_meses; mes++)
            {
              mon_inicial = mon_inicial * (1 + juros_mes);
             
              Console.WriteLine($"{mes}\tR${mon_inicial:F2}");
              Console.ReadLine();
            }


            





        }
    }
}
