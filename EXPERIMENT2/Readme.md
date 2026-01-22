 # experiment2
## TITLE: 2a.) Implement class mechanism in java 
```
class myclass {
void displaymessage() {
System.out.println("welcome to java");
}
int add (int a, int b) {
return a+b;
}
public static void main(String[] args) {
myclass obj = new myclass();
obj.displaymessage();
int result = obj.add(10, 20);
System.out.println("sum: " + result);
}
}
```
# output
<img width="1161" height="479" alt="2a output" src="https://github.com/user-attachments/assets/8738472c-05f1-44c5-b0da-a3f14ad111b7" />


# EXPERIMENT2B
## TITLE:2B.) java program implement method overloading
```
class OverloadExample {
int add(int a, int b) {
return (a + b);
}
double add(double a, double b) {
return a + b;
}
int add(int a, int b, int c) {
return a + b + c;
}
public static void main(String[] args) {
OverloadExample obj = new OverloadExample();
int sum1 = obj.add(10, 20);
double sum2 = obj.add(5.5, 6.5);
int sum3 = obj.add(10, 20, 30);
System.out.println("Result of adding two integers: " + sum1);
System.out.println("Result of adding two double values: " + sum2);
System.out.println("Result of adding three integers: " + sum3);
}
}
```
# output
<img width="1438" height="403" alt="2b output" src="https://github.com/user-attachments/assets/8290fba4-3a8d-42fe-a0c2-b559481ff55c" />


  # EXPERIMENT2C
  ## TITLE:2C.) java program implement constructor
  ```
class Student {
String name;
int age;
int marks;
Student (String n, int a, int m) {
name = n;
age = a;
marks = m;
}
void display (){ 
System.out.println ("Name: " + name);
System.out.println ("Age: " + age);
System.out.println ("Marks: " + marks);
}
public static void main(String[] args) {
Student S1 = new Student ("Alice", 20, 85);
S1.display ( );
}
}
```
# output
<img width="390" height="159" alt="2c output" src="https://github.com/user-attachments/assets/26423a2f-ac36-4cfc-85f0-5d6a352073d1" />




