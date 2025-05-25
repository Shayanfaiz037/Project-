import java.util.Scanner;

public class UnitConverterCentral {

public static void main(String[] args) {

Scanner scanner = new Scanner(System.in);

System.out.println("Welcome to Unit Converter Central!");

System.out.println("Choose the type of conversion:");

System.out.println("1. Celsius to Fahrenheit");

System.out.println("2. Kilometers to Miles");

System.out.println("3. Kilograms to Pounds");

System.out.print("Enter your choice (1-3): ");

int choice = scanner.nextInt();

switch (choice) {

case 1:

System.out.print("Enter temperature in Celsius: ");

double celsius = scanner.nextDouble();

double fahrenheit = (celsius * 9 / 5) + 32;

System.out.printf("%.2f°C is %.2f°F%n", celsius, fahrenheit);

break;

case 2:

System.out.print("Enter distance in kilometers: ");

double km = scanner.nextDouble();

double miles = km * 0.621371;

System.out.printf("%.2f km is %.2f miles%n", km, miles);

break;

case 3:

System.out.print("Enter weight in kilograms: ");

double kg = scanner.nextDouble();

double pounds = kg * 2.20462;

System.out.printf("%.2f kg is %.2f pounds%n", kg, pounds);

break;

default:

System.out.println("Invalid choice. Please select from 1 to 3.");

}

scanner.close();

}

}
