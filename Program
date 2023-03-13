//програма запитує користувача кількість змінних в таблиці істиності і залежно від цього будує табличку

namespace TruthTable
{
    internal class Program
    {
        static void TruthTable(int n) // Метод, який створює і виводить таблицю істинності
        {
            int rows = Convert.ToInt32(Math.Pow(2, n)); // обчислюємо кількість рядків у таблиці істинності
           
            for (int i = rows - 1; i >= 0; i--)
            {
                for (int j = 0; j < n; j++)
                {
                    // обчислюємо значення стовпця
                    int p = Convert.ToInt32(Math.Pow(2, n - j - 1));
                    bool value = (i / p) % 2 == 0;

                    // виводимо значення стовпця в рядку
                    Console.Write(value ? "1 " : "0 ");
                }
                Console.WriteLine();
            }
        }
        static void Main()
        {
            Console.OutputEncoding = Encoding.UTF8;

            Console.Write("Введіть кількість змінних: ");
            int n;
            n = Convert.ToInt32(Console.ReadLine());

            // викликаємо функцію для виведення таблиці істинності з n змінними
            TruthTable(n);

            Console.ReadKey();
        }
       
    }

}
