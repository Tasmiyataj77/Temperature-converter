# Temperature-converter
#include <iostream>
using namespace std;

// Function to convert Celsius to Fahrenheit
double celsiusToFahrenheit(double celsius) {
    return (celsius * 9.0 / 5.0) + 32.0;
}

// Function to convert Celsius to Kelvin
double celsiusToKelvin(double celsius) {
    return celsius + 273.15;
}

// Function to convert Fahrenheit to Celsius
double fahrenheitToCelsius(double fahrenheit) {
    return (fahrenheit - 32.0) * 5.0 / 9.0;
}

// Function to convert Fahrenheit to Kelvin
double fahrenheitToKelvin(double fahrenheit) {
    return (fahrenheit - 32.0) * 5.0 / 9.0 + 273.15;
}

// Function to convert Kelvin to Celsius
double kelvinToCelsius(double kelvin) {
    return kelvin - 273.15;
}

// Function to convert Kelvin to Fahrenheit
double kelvinToFahrenheit(double kelvin) {
    return (kelvin - 273.15) * 9.0 / 5.0 + 32.0;
}

int main() {
    int choice;
    double temperature;

    cout << "Temperature Converter" << endl;
    cout << "1. Celsius to Fahrenheit" << endl;
    cout << "2. Celsius to Kelvin" << endl;
    cout << "3. Fahrenheit to Celsius" << endl;
    cout << "4. Fahrenheit to Kelvin" << endl;
    cout << "5. Kelvin to Celsius" << endl;
    cout << "6. Kelvin to Fahrenheit" << endl;

    cout << "\nEnter your choice: ";
    cin >> choice;

    // Prompt user to enter the temperature based on their conversion choice
    switch (choice) {
    case 1:
        cout << "\nEnter temperature in Celsius: ";
        cin >> temperature;
        cout << "Temperature in Fahrenheit: " << celsiusToFahrenheit(temperature) << "°F" << endl;
        break;
    case 2:
        cout << "\nEnter temperature in Celsius: ";
        cin >> temperature;
        cout << "Temperature in Kelvin: " << celsiusToKelvin(temperature) << "K" << endl;
        break;
    case 3:
        cout << "\nEnter temperature in Fahrenheit: ";
        cin >> temperature;
        cout << "Temperature in Celsius: " << fahrenheitToCelsius(temperature) << "°C" << endl;
        break;
    case 4:
        cout << "\nEnter temperature in Fahrenheit: ";
        cin >> temperature;
        cout << "Temperature in Kelvin: " << fahrenheitToKelvin(temperature) << "K" << endl;
        break;
    case 5:
        cout << "\nEnter temperature in Kelvin: ";
        cin >> temperature;
        cout << "Temperature in Celsius: " << kelvinToCelsius(temperature) << "°C" << endl;
        break;
    case 6:
        cout << "\nEnter temperature in Kelvin: ";
        cin >> temperature;
        cout << "Temperature in Fahrenheit: " << kelvinToFahrenheit(temperature) << "°F" << endl;
        break;
    default:
        cout << "Invalid choice!" << endl;
    }

    return 0;
}
