# Lab-10.40
#include <iostream>
#include <iomanip>
using namespace std;

int main() {
cout << setprecision(2) << fixed;
double total;
double shirts;
double discount;


 cout << "How many shirts would you like?" << endl;
 cin >> shirts;
 
 total = 12 * shirts;
 if (( shirts > 0 ) && (shirts <= 5 )) { 
   cout << "The cost per a shirt is $12 and the total cost is $" << total << endl;
}
 else if ((shirts >= 5) && (shirts <= 10)) {
   discount = total * .10;
   cout << "The cost per a shirt is $12 and the total cost is $" << total - discount  << endl;
 }
else if ((shirts >= 11) && (shirts <= 20)) {
  discount = total * .15;
  cout << "The cost per a shirt is $12 and the total cost is $" << total - discount << endl;
}
else if ((shirts >= 21) && (shirts <= 30)) {
  discount = total * .20;
  cout << "The cost per a shirt is $12 and the total cost is $" << total - discount << endl;
}
else if (shirts >= 31) {
  discount = total * .25;
  cout << "The cost per a shirt is $12 and the total cost is $" << total - discount << endl;
}
else 
  cout << "Invalid Input: Please enter a nonnegative integer" << endl;
 

}
