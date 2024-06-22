# lecture-8---cipher-schools-
In this lecture i learned how to reverse an array and and access and multiple inputs here is an sample program 
#include <iostream>

int main() {
    const int SIZE = 5;  // Define the size of the array
    int numbers[SIZE];   // Declare an array of integers

    // Prompt the user for input
    std::cout << "Enter 5 numbers:" << std::endl;
    for (int i = 0; i < SIZE; ++i) {
        std::cout << "Enter number " << (i + 1) << ": ";
        std::cin >> numbers[i];
    }

    // Reverse the array
    for (int i = 0; i < SIZE / 2; ++i) {
        int temp = numbers[i];
        numbers[i] = numbers[SIZE - 1 - i];
        numbers[SIZE - 1 - i] = temp;
    }

    // Print the reversed array
    std::cout << "The reversed array is:" << std::endl;
    for (int i = 0; i < SIZE; ++i) {
        std::cout << "Number " << (i + 1) << ": " << numbers[i] << std::endl;
    }

    return 0;
}
