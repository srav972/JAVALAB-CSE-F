# experiment6
## TITLE:6A.)EXPECTATION HANDLING MECHANISM
```
import java.util.Scanner;
public class ArrayExceptionDemo {
    public static void main(String[] args) {       
        Scanner sc = new Scanner(System.in);      
        System.out.print("Enter the size of the array: ");
        int n = sc.nextInt();   
        int[] arr = new int[n];
        System.out.println("Enter " + n + " elements:");
        for(int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        System.out.print("Enter index to access: ");
        int index = sc.nextInt();
        try {
            System.out.println("Element at index " + index + " is: " + arr[index]);
        } 
        catch(ArrayIndexOutOfBoundsException e) {
            System.out.println("Invalid index! Please enter index between 0 and " + (n-1));
        }
        
        sc.close();
    }
}
```
# OUTPUT
<img width="279" height="76" alt="6A" src="https://github.com/user-attachments/assets/f4c13f72-5dd4-4af7-90a0-432d798cf20e" />


# experiment6
## TITLE:6b)illustrsting multiple catch clauses
```
import java.util.Scanner;

public class ArrayExceptionDemo {
    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);
        
        // Read size of array
        System.out.print("Enter the size of the array: ");
        int n = sc.nextInt();
        
        int[] arr = new int[n];
        
        // Read array elements
        System.out.println("Enter " + n + " elements:");
        for(int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        
        // Ask user for index
        System.out.print("Enter index to access: ");
        int index = sc.nextInt();
        
        // Exception handling
        try {
            System.out.println("Element at index " + index + " is: " + arr[index]);
        } 
        catch(ArrayIndexOutOfBoundsException e) {
            System.out.println("Invalid index! Please enter index between 0 and " + (n-1));
        }
        
        sc.close();
    }
}
```
# output
<img width="323" height="62" alt="6B" src="https://github.com/user-attachments/assets/eef1d8d5-4952-4c1b-ae29-7549e608311b" />


# experiment6
## TITLE:6c.)java built -in expexction
```
import java.util.Scanner;
public class BuiltInExceptionDemo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        try {

            System.out.print("Enter an integer to divide 100: "$
            int n = sc.nextInt();
            int result = 100 / n;
            System.out.println("Result: " + result);


            int[] arr = new int[3];
            System.out.println("Accessing element at index 5: "$

              sc.nextLine();
            System.out.print("Enter a number as text: ");
            String s = sc.nextLine();
            int num = Integer.parseInt(s);
            System.out.println("Converted number: " + num);
        }

        catch (ArithmeticException e) {
            System.out.println("ArithmeticException: Division b$
        }

catch (ArithmeticException e) {
            System.out.println("ArithmeticException: Division b$
        }

        catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("ArrayIndexOutOfBoundsException:$
        }
              
        catch (NumberFormatException e) {
            System.out.println("NumberFormatException: Invalid $
        }
            
        catch (Exception e) {
            System.out.println("Some other exception occurred."$
        }
            
        System.out.println("Program continues...");

        sc.close();
    }
}
```
# output
<img width="318" height="47" alt="6C" src="https://github.com/user-attachments/assets/700f4508-74ba-426d-9644-862a6963988b" />

<img width="403" height="62" alt="6c-2" src="https://github.com/user-attachments/assets/b9dd48a1-db64-4514-b0a0-3f6defb04e94" />
        
