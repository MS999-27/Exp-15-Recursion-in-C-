# AIM
To learn about recursion in c++.

# Problem Statement
1.) Write a c++ program to get factorial of a number using recursion.

2.) Write a c++ program to find fibonacci number in the fibonacci sequence using recursion.

3.) Write a c++ program to find sum of n natural numbers using recursion.

# Theory

Recursion is the technique of making a function call itself. This technique provides a way to break complicated problems down into simple problems which are easier to solve.

Recursion may be a bit difficult to understand. The best way to figure out how it works is to experiment with it.


# Problem Codes
```javascript


//FACTORIAL
# include<iostream>
using namespace std;
 int factorial (int n)
{ if ( n == 0)
{
    return 1;
}
else 
{
    return n*factorial(n-1);
    }
    }
    int main()
    {  int num;
       cout<<"Enter a number: "<<endl;
       cin>>num;

       cout<<"The factorial of "<<num<<" is: "<< factorial(num)<<endl;
       return 0;
    }

//FIBONACCI SEQUENCE
# include<iostream>
using namespace std;
int fib(int n)
{
    if(n==0)
    {
        return 0;
    }
    if(n==1)
    {
        return 1;
    }
    else
    {
     return (fib(n-1) + fib(n-2));
    }

}
int main()
{
    int f,n;
    cout << "Enter number of elements: "<<endl;
    cin >> n ;

    cout << n <<"th Fibonacci number in Fibonacci sequence is: "<<fib(n) ;
 
}

//SUM OF 'n'  NATURAL NUMBERS
# include<iostream>
using namespace std;
int sum(int n)
{
    if(n==0)
    {
        cout<< " Number should be greater than 1"<<endl;
    }
    if(n==1)
    {
        return 1;
    }
    else
    {
     return (n+sum(n-1));

    }
}
    int main()
{
    int f,n;
    cout << "Enter a number : "<<endl;
    cin >> n ;

    cout << n <<"Sum of numbers from 1 to "<<n<<" is: "<<" : "<<sum(n) ;
 
}
```
# Output
## Factorial
![Exp 15 Factorial](https://github.com/user-attachments/assets/2d5074b9-2213-4bfe-9211-91b3e46516c1)

## Fibonacci Sequence
![Exp 15-Fibonnacci](https://github.com/user-attachments/assets/f4549c04-68be-4cdc-b08e-745a60ef140b)

## Sum of 'n' natural numbers
![Exp 15 natural numsum](https://github.com/user-attachments/assets/e025f2b4-ad7d-4dea-9974-4ab9e826b716)
# Conclusion

We learnt to find factorial, fibonacci sequence and sum of 'n' natural numbers using recursion.


