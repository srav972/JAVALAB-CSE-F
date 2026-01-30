# experiment add3
## TITLE:3) STRING IS PALINDROME OR NOT
```
import java.util.Scanner;

public class PalindromeString {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a string: ");
        String str = sc.nextLine();
        String reverse = "";
        for (int i = str.length() - 1; i >= 0; i--) {
            reverse = reverse + str.charAt(i);
        }
        if (str.equals(reverse)) {
            System.out.println("The string is a Palindrome");
        } else {
            System.out.println("The string is NOT a Palindrome");
        }
        sc.close();
    }
}
```
# OUTPUT
<img width="358" height="31" alt="3A ADD OUTPUT" src="https://github.com/user-attachments/assets/3f7edd39-10d4-47c7-b774-f9218f30cfed" />
