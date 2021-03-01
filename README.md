#include <iostream>
using namespace std;

class amountClass
{
    public:
        double getTax(double x)
        {
            double taxrate = .08;
            double total = 0;
            total+=(taxrate*x+x);
            totalprice = total;
            return totalprice;
        }
        void getPrice()
        {
            cout << "Your price is " << totalprice << endl;
        }
    private:
        double totalprice;
};

int main()
{
    double initialPrice;
    cout << "This program allows you to calculate the final taxed price of a product with an 8% tax rate" << endl;
    cout << "Please enter the price of the product: ";
    cin >> initialPrice;
    amountClass taxobject;
    taxobject.getTax(initialPrice);
    taxobject.getPrice();
    return 0;
}
