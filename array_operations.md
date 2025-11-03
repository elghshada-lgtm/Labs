// Name: Shada Elghariani
// Course: CISC 192 C++ Programming 
// Date: 11/02/2025
// Assignment: Arrays 

#include <iostream>
#include <array>

using namespace std;

int main () {
  const int N = 5; // This is the Array size 
  array<int, N> numbers{};

  cout << "Enter " << N << " unique integers: \n";

  for (int i = 0; i < N; i++) {
    bool duplicate;
    do{
      duplicate = falsa
      cout << "Element " << i +1 << ": ";
      cin >> numbers[i];

      // checking for duplicates 
      for  (int j = 0; j < i; j++) {
        if (numbers[i] == numbers [j]) {
        cout << "DUplicate Found! Enter a different number. \n";
        duplicate = true;
        break;
      }
    }
  } while (duplicate);
}

cout << "\nChoose an operation: \n";
Cout << "1. Sort in Ascending order\n";
cout << "2. Sort in Descending order\n";
cout << "3. Find the Maximum Number\n";
cout << "Enter your choise: ";

int choice; 
cin >> choice;

switch (choise) {
  case 1: {
    // Sort in Ascending order:
    for (int i = 0; i < N -1; i++) {
      for (int j = 0; j < n - i - 1; j++) {
        if (numbers [j] > numbers [j + 1] {
          int temp = numbers[j];
          numbers[j] = numbers[j + 1];
          number[j + 1] = temp;
        }
      }
    }
    cout << "\nArray sorted in ascending order: \n";
    for (int num : numbers)
      cout << num << " ";
    cout << endl;
    break;
  }

  case 2: {
    // Sort in Descedning order
    for (int i = 0; i < N -1; i++) {
      for (int j = 0; j < n - i - 1; j++) {
        if (numbers [j] < numbers [j + 1] {
          int temp = numbers[j];
          numbers[j] = numbers[j + 1];
          number[j + 1] = temp;
        }
      }
    }
    cout << "\nArray sorted in descending order: \n";
    for  (int num : numbers)
      cout << num << " ";
    cout << endl;
    break;
  }

  case 3: {
    int max = numbers[0];
    for (int i = 1; i < N; i++) {
      if (numbers[i] > max)
        max = numbers[i];
    }
    cout << "\nThe maximum number is: " << max << endl;
    break;
  }

  defult:  
    cout << "Invalud choice, please try again. \n";
}

return 0;
