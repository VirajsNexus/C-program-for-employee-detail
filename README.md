# C-program-for-employee-detail

//EXP:2
//Name:Viraj Jamdhade
//Div : A
//Roll No. : 67

//Write a Program to calculate total salary and display Employee detail

#include<iostream>
#include<string>
using namespace std;
class Employee
{
public:
    //Data Member
    string name;
    int id;
    float basic_salary;
    float bonus;

    float calculatetotalSalary()  // Function to calculate Total Salary
    {
        return basic_salary + bonus;
    }
    //Function to Display Employee Details
    void displayEmployeedetails()
    {
         cout<<"Employee ID:" <<id<<endl;
         cout<<"Name:" <<name<<endl;
         cout<<"Basic Salary:" <<basic_salary<<endl;
         cout<<"Bonus:" <<bonus<<endl;
         cout<<"Total Salary:" <<calculatetotalSalary()<<endl;
    }
};
int main()
{
    //Create an Object of Employee Class
    Employee emp1,emp2;
    //Take input for  Details
    cout<<"Enter 1st Employee Details:"<<endl;
    cout<<"Enter Employee ID:";
    cin>>emp1.id;
    cout<<"Enter Employee Name:";
    cin>>emp1.name;
    cout<<"Enter Basic Salary:";
    cin>>emp1.basic_salary;
    cout<<"Enter Bonus:";
    cin>>emp1.bonus;
    emp1.displayEmployeedetails();

    cout<<"----------------------------------------------"<<endl;
   //Take Employee Details for second employee
    cout<<"Enter 2nd Employee Details:"<<endl;
    cout<<"Enter Employee ID:";
    cin>>emp2.id;
    cout<<"Enter Employee Name:";
    cin>>emp2.name;
    cout<<"Enter Basic Salary:";
    cin>>emp2.basic_salary;
    cout<<"Enter Bonus:";
    cin>>emp2.bonus;
    emp2.displayEmployeedetails();
}
