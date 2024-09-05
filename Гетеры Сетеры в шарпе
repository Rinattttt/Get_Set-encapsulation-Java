using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace laba10
{
    class Program
    {
        static void Main(string[] args)
        {
            Students Student1 = new Students("Фельдман Г.И", 2023, "г. Пенза", 89998285698, 1, "Информационные технологии");
            Students Student2 = new Students("Исаев И.Н", 2021, "г. Москва", 89998896452, 3, "Экономика");
            Students Student3 = new Students("Петров Н.В", 2022, "г. Рязань", 88005553535, 2, "Агрономия");
            Students[] massiv = new Students[3] { Student1, Student2, Student3 };
            Console.WriteLine("ФИО всех студентов:");
            for (int i = 0; i<3; i++)
            {
                Console.WriteLine(massiv[i].FIO_Property);
            }
            Console.WriteLine("Список студентов указанного факультета:");
            for (int i = 0; i < 3; i++)
            {
                if (massiv[i].Faculty_Property == "Экономика")
                {
                    Console.WriteLine(massiv[i].FIO_Property);
                }
            }
            Console.WriteLine("Список студентов, поступивших после указанного года:");
            for (int i = 0; i < 3; i++)
            {
                if (massiv[i].Date_Property > 2021)
                {
                    Console.WriteLine(massiv[i].FIO_Property);
                }
            }
            Console.ReadKey();
        }
    }
    class Students
    {
        private string FIO;// get set
        private int Date;//set
        private string Address;//get
        private long Phone_number;//get set
        private int Course;//set
        private string Faculty;//get
        public string FIO_Property
        {
            get { return FIO; }
            set { FIO = value; }
        }
        public int Date_Property
        {
            get { return Date; }
            set { Date = value;}
        }
        public string Address_Property
        {
            get { return Address; }
        }
        public long Phone_number_Property
        {
            get { return Phone_number; }
            set { Phone_number = value; }
        }
        public int Course_Property
        {
            set { Course = value; }
        }
        public string Faculty_Property
        {
            get { return Faculty; }
        }
        public Students(string FIO, int Date, string Address, long Phone_number, int Course, string Faculty)
        {
            this.FIO = FIO;
            this.Date = Date;
            this.Address = Address;
            this.Phone_number = Phone_number;
            this.Course = Course;
            this.Faculty = Faculty;
        }
    }
}
