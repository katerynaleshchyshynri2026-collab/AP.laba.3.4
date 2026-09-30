#include <iostream>

using namespace std;

int main()
{
    double x;    // координата x
    double y;    // координата y
    double R1;   // внутрішній радіус
    double R2;   // зовнішній радіус

    cout << "R1 = "; cin >> R1;
    cout << "R2 = "; cin >> R2;
    cout << "x = "; cin >> x;
    cout << "y = "; cin >> y;

    // розгалуження в повній формі
    if (((R1 * R1 <= x * x + y * y) &&
        (x * x + y * y <= R2 * R2) &&
        (x >= 0) && (y >= 0)) ||
        ((R1 * R1 <= x * x + y * y) &&
            (x * x + y * y <= R2 * R2) &&
            (x <= 0) && (y <= 0)))

        cout << "yes" << endl;
    else
        cout << "no" << endl;

    cin.get();
    cin.get();

    return 0;
}
