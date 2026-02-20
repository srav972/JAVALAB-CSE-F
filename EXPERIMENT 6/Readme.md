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
