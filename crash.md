#include <iostream>
using namespace std;
class ZeroObj
{
public:
    ZeroObj();
    ~ZeroObj();
    void say_hello()
    {
        cout<<"hello this say_hello"<<endl;
    }

    void say_my_secret(int id)
    {
        m_id = id;
        cout <<"my secret id is  "<<m_id<<endl;
    }

private:
    int m_id;
};
void test1(void)
{
    ZeroObj *pObj = NULL;
    
    pObj->say_hello();
}
void test2(void)
{
    ZeroObj *pObj = NULL;
    
    pObj->say_my_secret(1);
}
int  main(int argc, char const *argv[])
{
    test1();
    test2();
    return 0;
}
