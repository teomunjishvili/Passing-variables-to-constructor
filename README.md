#include<iostream>
#include<string>
using namespace std;

class Person
{
    /*private variables*/
        string firstname;
        string lastname;
        int telephoneNumber;
    public:
        /*there is no variable passed to the constructor*/
        Person()
        {
            firstname = "Nick";
            lastname = "Akkerer";
            telephoneNumber = 599974546;
        }
        
        /*only one variable is passed to the constructor*/
        Person(string a)
        {
            firstname = a;
            lastname = "Metonidze";
            telephoneNumber = 598666667;
        }
        
        
        /*two variables are passed to the constructor*/
        Person(string a, string b)
        {
            firstname = a;
            lastname = b;
            telephoneNumber = 596100009;
        }
        
        void get_values()
        {
            cout<<"Firstname: "<<firstname<<endl;
            cout<<"Lastname: "<<lastname<<endl;
            cout<<"Telephone Number: "<<telephoneNumber<<endl;
        }
};

int main ()
{
    Person obj1, obj2("Natia"), obj3("Mariam", "Kajaia");
    obj1.get_values();
    obj2.get_values();
    obj3.get_values();
    
    return 0;
}
