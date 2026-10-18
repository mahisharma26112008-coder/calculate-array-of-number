# calculate-array-of-number

#include <iostream>
using namespace std;

int main()
{
    int a[5], i, sum = 0, choice;
    float avg;

    cout << "Enter 5 elements:\n";
    for (i = 0; i < 5; i++)
    {
        cin >> a[i];
    }

    cout << "1. Calculate Average";
    cout << "\nEnter your choice: ";
    cin >> choice;

    switch (choice)
    {
        case 1:
            for (i = 0; i < 5; i++)
            {
                sum = sum + a[i];
            }

            avg = (float)sum / 5;

            cout << "Average = " << avg;
            break;

        default:
            cout << "Invalid choice";
    }

    return 0;
}
