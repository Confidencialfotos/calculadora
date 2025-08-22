using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using static System.Console;

namespace ConsoleApp3
{
    internal class Program
    {
        static void Main(string[] args)
        {
            char op;
            float num1, num2, resultado;
            WriteLine("Digite o primeiro número: ");
            num1 = Convert.ToSingle(ReadLine());
            WriteLine("Digite o segundo numero: ");
            num2 = Convert.ToSingle(ReadLine());
            WriteLine("Digite a operação (+,-,*,/): ");
            op = Convert.ToChar(ReadLine());
            switch (op)
            {
                case '*':
                    resultado = num1 + num2;
                    WriteLine("{0} * {1} = {2}", num1, num2, resultado);
                    break;

                case '/':
                    resultado = num1 / num2;
                    WriteLine("{0} / {1} = {2}", num1, num2, resultado);
                    break;

                case '+':
                    resultado = num1 + num2;
                    WriteLine("{0} + {1} = {2}", num1, num2, resultado);
                    break;

                case '-':
                    resultado = num1 - num2;
                    WriteLine("{0} - {1} = {2}", num1, num2, resultado);
                    break;

                default:
                    WriteLine("Operação inválida!");
                    break;
            }
                                       
            ReadKey();

        }

    }
}
