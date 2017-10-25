
    using System;
namespace Fibonacci_Solucion

{

    class Program
    
    {
    
        static void Main(string[] args)
        
        
        {
            Console.WriteLine("Ingrese la cantidad de valores que de la serie que desea ver:");
            
            int n = Convert.ToInt32(Console.ReadLine());
            
            int a = Fibo(n);   //Llama a la funcion "Fibo" junto a la variable que ingreso el usuario
            
        }
        
        
        static int Fibo(int numero)  //Ejecuta la funcion y reemplaza "n" con "numero"
        
        {
        
            int x = 0;
            
            int y = 1;
            
            int serie;   
            
            for (int i = 0; i < numero; i++)
            {
                serie = x;
                
                x = y;
                
                y = serie + x;
                
                numero = x;
                
                Console.WriteLine(x);  //Muestra la serie directamente en la funcion
            }
            Console.ReadKey();
            
            return numero;     //Retorna la variable que se ingreso para que termine la funcion
          
        }
      }
    }
