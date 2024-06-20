using System;
using System.Collections.Generic;

namespace TaxiInfo
{
    // Класс для хранения информации о водителе
    public class Driver
    {
        public string FirstName { get; set; }
        public string LastName { get; set; }
        public string CarNumber { get; set; }
        public string CarModel { get; set; }

        // Конструктор для инициализации данных водителя
        public Driver(string firstName, string lastName, string carNumber, string carModel)
        {
            FirstName = firstName;
            LastName = lastName;
            CarNumber = carNumber;
            CarModel = carModel;
        }
    }

    class Program
    {
        static void Main(string[] args)
        {
            // Список водителей такси класса "Эконом"
            List<Driver> economyDrivers = new List<Driver>
            {
                new Driver("Иван", "Иванов", "A123BC", "Hyundai Solaris"),
                new Driver("Петр", "Петров", "B456CD", "Kia Rio"),
                new Driver("Алексей", "Алексеев", "D012EF", "Ford Focus")
            };

            // Список водителей такси класса "Комфорт"
            List<Driver> comfortDrivers = new List<Driver>
            {
                new Driver("Сергей", "Сергеев", "C789DE", "Toyota Camry"),
                new Driver("Дмитрий", "Дмитриев", "E345FG", "Mercedes E-Class")
            };

            // Вывод информации о водителях класса "Эконом"
            Console.WriteLine("Водители такси класса 'Эконом':")

foreach (var driver in economyDrivers) { Console.WriteLine ("Имя: {driver.FirstName}, Фамилия: {driver.LastName}, Номер машины: {driver.CarNumber}, Модель машины: {driver.CarModel}");
