#include<iostream>
#include<iomanip>
#include<cctype>


using namespace std;


int main()


{
   //variable delcerations
   int radius;
   double volume;
   char again;
  
   //begin do while loop
   do {
  
       //code to execute initially, and every time they enter y or Y after execution
   cout << "enter the radius of a sphere: ";
   cin >> radius;
   volume = 1.3333*3.1416*radius*radius*radius;
  
   cout << "the volume of the sphere is " << fixed << setprecision(1) << volume << endl;
  
   cout << "would you like to calculate another sphere volume? (y/n): ";
   cin >> again;
   again = tolower(again);
  
   } while (again == 'y');
  
       //if user does not enter y or Y, done
  
  return 0;
 
  
  }
