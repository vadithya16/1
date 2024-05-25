1a:
class Test1a
{
int a;
Test1a()
{
a=1;
}
Test1a(int i)
{
a=i;
}
void show()
{
System.out.println("\n Value of a : " +a);
}
void show(int m)
{
System.out.println("\n Value of argument passed : " +m);
}
}
class Q1a
{
public static void main(String args[])
{
Test1a ob1=new Test1a();
Test1a ob2=new Test1a(10);
ob1.show();
ob2.show();
ob2.show(33);
}
}

1b:
class Outer
{
int x=100;
int y=10;
void test()
{
Inner ob1=new Inner();
ob1.display();
}
class Inner
{
int z;
Inner()
{
y=90;
z=60;
}
void display()
{
System.out.println("Display : x = " +x);
System.out.println("Display : y = " +y);
System.out.println("Display : z = " +z);
}
}
void show()
{
System.out.println("Display : x = " +x);
Department of M.C.A Page 6 of 26
System.out.println("Display : y = " +y);
}
}
class Q1b
{
public static void main(String args[])
{
Outer ob1=new Outer();
ob1.test();
ob1.show();
}
}
