#include<bits/stdc++.h>
using namespace std;
class student{
private:
    int a;
public:
    student(int x)
    {
        a=x;
    }
    friend void show(student j);
};
void show(student o)
{
    cout<<"this is a friend function"<<endl<<o.a;
}
int main()
{
    student ob(10);
    show(ob);
}
