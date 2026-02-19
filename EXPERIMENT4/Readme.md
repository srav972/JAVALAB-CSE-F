# experiment4a
##  TITLE:4a.)SINGLE INHERITANCE
```
public class Person {
    String name;
    int age;  
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }
    public void displayPersonDetails() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
    }
}
public class Employee extends Person {
    double annualSalary;
    int yearOfJoining;
    String nationalInsuranceNumber;
    public Employee(String name, int age, double annualSalary,
                    int yearOfJoining, String nationalInsuranceNumber) {
        super(name, age);
        this.annualSalary = annualSalary;
        this.yearOfJoining = yearOfJoining;
        this.nationalInsuranceNumber = nationalInsuranceNumber;
    }
    public void displayEmployeeDetails() {
        displayPersonDetails();
        System.out.println("Annual Salary: " + annualSalary);
        System.out.println("Year Of Joining: " + yearOfJoining);
        System.out.println("National Insurance Number: " + nationalInsuranceNumber);
    }
}
public class TestEmployee {
    public static void main(String[] args) {
        Employee emp1 = new Employee(
                "Rahul Sharma",
                30,
                550000.00,
                2021,
                "NI123456A"
        );
        emp1.displayEmployeeDetails();
    }
}
```
# OUTPUT
<img width="323" height="121" alt="4A" src="https://github.com/user-attachments/assets/77debd17-1fbe-4623-a553-edae5adddeb4" />


# experiment4b
##  TITLE:4b.)Multi-level inheritance
```
class Bicycle {
    String pedalType;
    void showBicycleInfo() {
        System.out.println("This is a bicycle with pedals.");
        System.out.println("Pedal Type: " + pedalType);
    }
}
class Motorbike extends Bicycle {
    int engineCapacity;
    void showMotorbikeInfo() {
        System.out.println("This motorbike has an engine.");
        System.out.println("Engine Capacity: " + engineCapacity + " cc");
    }
}
class ElectricBike extends Motorbike {
    int batteryCapacity;
    void showElectricBikeInfo() {
        System.out.println("This electric bike has an electric motor and battery.");
        System.out.println("Battery Capacity: " + batteryCapacity + " Wh");
    }
}
public class TestVehicle {
    public static void main(String[] args) {
        ElectricBike eBike = new ElectricBike();
        eBike.pedalType = "Standard Pedals";
        eBike.engineCapacity = 150;
        eBike.batteryCapacity = 500;
        eBike.showBicycleInfo();
        eBike.showMotorbikeInfo();
        eBike.showElectricBikeInfo();
    }
}
```
# output
<img width="499" height="132" alt="4b" src="https://github.com/user-attachments/assets/b08ed3ed-85da-48cb-9350-c46ac76357cb" />


# experiment4a
##  TITLE:4c.)abstract class
```
abstract class Figure {
    double dim1;
    double dim2;
    Figure(double dim1, double dim2) {
        this.dim1 = dim1;
        this.dim2 = dim2;
    }
    abstract double area();
}
class Rectangle extends Figure {
    Rectangle(double length, double breadth) {
        super(length, breadth);
    }
    double area() {
        return dim1 * dim2;
    }
}
class Triangle extends Figure {
    Triangle(double base, double height) {
        super(base, height);
    }
    double area() {
        return 0.5 * dim1 * dim2;
    }
}
public class TestFigure {
    public static void main(String[] args) {
     Figure f1 = new Rectangle(10, 5);
        System.out.println("Area of Rectangle = " + f1.area());
        Figure f2 = new Triangle(8, 4);
        System.out.println("Area of Triangle = " + f2.area());
    }
}
```
# output
<img width="242" height="44" alt="4c" src="https://github.com/user-attachments/assets/095bf57a-7975-43ec-8b2a-d9b4a23aa5ee" />

