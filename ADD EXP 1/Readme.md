# experiment add1
## TITLE:1) INSERT SUB STRING
```
import java.util.Scanner;
public class InsertSubstring {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the main string: ");
        String mainString = sc.nextLine();
        System.out.print("Enter the substring to insert: ");
        String subString = sc.nextLine();
        System.out.print("Enter the position to insert the substring: ");
        int position = sc.nextInt();
        String result = mainString.substring(0, position) 
                        + subString 
                        + mainString.substring(position);
        System.out.println("String after insertion: " + result);
        sc.close();
    }
}
```
# OUTPUT
<img width="289" height="58" alt="1 ADD OUTPUT" src="https://github.com/user-attachments/assets/cf3d849f-57e2-4976-aff5-9cc7d1469b06" />


# experiment add3
## TITLE:1) STRING IS PALINDROME OR NOT
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
<img width="358" height="31" alt="3A ADD OUTPUT" src="https://github.com/user-attachments/assets/c9ce1493-bee4-4081-b961-829bcd90cdd1" />
