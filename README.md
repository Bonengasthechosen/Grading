# Grading
Using stack overflow for grading and comments of the accepted data  of five subjects including their average
#include <iostream>

using namespace std;

int main()
{
    //Variables declaration.
    int sub1,sub2,sub3, sub4,sub5,total,avg;

    //accepting marks from user in each subject
    cout << " Enter English Marks: " << endl;
    cin >> sub1;
    cout << " Enter Kiswahili Marks : " << endl;
    cin >> sub2;
    cout << " Enter GHC Marks : " << endl;
    cin >> sub3;
    cout << " Enter Maths Marks: " << endl;
    cin >> sub4;
    cout << " Enter science Marks: " << endl;
    cin >> sub5;

    //calculating sum of marks obtained in each subject
    total = (sub1 + sub2 + sub3 + sub4 + sub5);

    //calculating the average marks
    avg = total / 5;

    // Beginning of if condition to find out grades of total subjects.

    switch (avg){
      case 1:{
        if ((avg >= 80) && (avg <= 100))
        {
            cout << " Your Average is: " << avg << endl;
            cout << "You Grade is A+ " << endl;
        }
        break; 
      }
      case 2:{
        if ((avg >= 70) && (avg <= 79))
        {
            cout << " Your Average is: " << avg << endl;
            cout << " Your grade is A " << endl;
        }    
        break;
      } 
      case 3:{
        if ((avg >= 60) && (avg <= 69))
        { 
            cout << " Your Average is: " << avg << endl;
            cout << " Your Grade is B+  " << endl;
        }   
        break;  
      }
      case 4:{ 

        if ((avg >= 50) && (avg <= 59))
        {
            cout << " Your Average is: " << avg << endl;
            cout << " Your Grade is C+ " << endl;
        }
        break;
      }
      case 5: {
        if ((avg >= 40) && (avg <= 49))
        {
            cout << " Your Average is: " << avg << endl;
            cout << " Your Grade is  C- ! " << endl;
        }
        break;    
      }
      case 6: {
        if ((avg >= 30) && (avg <= 39))
        {
            cout << " Your Average is: " << avg << endl;
            cout << " Your Grade is  D ! " << endl;
        }
        break; 
      }

      default:{ 
        if ((avg >= 100) && (avg <= 29))
        {
            cout << " Your Average is: " << avg << endl;
            cout << " Your Grade is  F, So you are Fail in the class ! " << endl;
            break;
        }
      }
    }

    system("pause");
}



