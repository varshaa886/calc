#include <iostream>

using namespace std;


double pow(double basen,int pown)
{
    double result=1.0;
    for(int i=0;i<pown;i++)
    {
        result=result*basen;
        
    }
    return result;
}

int fact(int num)
{
    int f,c;
    for(f=c=1;num>=c;num--)
    {
        f=f*num;
    }
    return f;
}
double sine(double x) 
{
    double result = 0.0;
    for (int n = 0; n < 10; ++n) 
    {
        result += pow(-1, n) * pow(x, 2 * n + 1) / fact(2 * n + 1);
    }
    return result;
}
double cosine(double x)
{
    double result = 0.0;
    for (int n = 0; n < 10; ++n) 
    {
        result += pow(-1, n) * pow(x, 2 * n) / fact(2 * n);
    }
    return result;
}

double exponent(double x)
{
    double result=0.0;
    for (int n=0;n<10;n++)
    {
        result+= pow(x,n) / fact(n);
    
    }
    return result;
}
int main(){
char choice,trig;
double angle,rad;
char ch;
int n,i,num1,num2,basen,pown,num;
cout<< "Type of operation(Algebraic- A/Trignometric-T/Exponent-E)";
cin>> choice;
if (choice == 'A' || choice == 'a')
{
cout << "enter the operator(+,-,*,/,^,!)";
cin>> ch;
if(ch=='+' || ch=='-' || ch=='*'|| ch=='/')
{
cout << "Enter value of num1: ";
cin >> num1;
cout << "Enter value of num2: ";
cin >> num2;
}
else if(ch=='^')
{
cout << "Enter the base number: ";
cin >> basen;
cout << "Enter the power number: ";
cin >> pown;
}
switch(ch)
{
case '+':
cout << "Sum of the numbers is: " << num1+num2 <<endl;
break;
case '-':
cout << "Diffrence of the numbers is: " << num1-num2<< endl;
break;
case '/':
if(num2==0)
{
    cout<<"Error!Division by zero";
}
else
{
cout << "Division of the numbers is: " << num1/num2 <<endl;
}
break;
case '*':
cout << "Product of the numbers is: " << num1*num2 << endl;
break;
case '^':
cout<<"Base to the power is: " ;
cout << pow(basen,pown);
break;
case '!':
cout << "Enter the number of which you want factorial:";
    cin>> num;
    cout<<"The factorial of the given number is";
    cout<< fact(num);
    break;

default:
cout<<"Invalid operator";
}
}
else if(choice=='E' || choice == 'e')
{
    double num;
    cout<<"Enter the exponent:";
    cin>>num;
    cout<<exponent(num);
}
else if(choice == 'T' || choice == 't')
{
    cout<< "select the trignometric function(sin-s/cos-c): ";
    cin>> trig;
    if(trig == 's' || trig== 'c')
    {
        cout<< "Enter the angle in degrees: ";
        cin >> angle;
    }
    rad=(3.14*angle)/180;
}
double x;
  x=rad;
if (trig == 's')
{
   cout << "Result: " << sine(rad) << endl;
}
else if(trig=='c')
{
    cout<<cosine(rad)<<endl;
}
else
{
    cout<<"Invalid operator";
}


return 0;
}
