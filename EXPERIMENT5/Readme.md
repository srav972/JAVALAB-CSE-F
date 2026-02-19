# experiment5
## title:5a.)implement interface
```
interface Sortable {
    void sort(int[] arr);
}
class BubbleSort implements Sortable {
    public void sort(int[] arr) {
        int n = arr.length;
        for (int i = 0; i < n - 1; i++) {
            for (int j = 0; j < n - i - 1; j++) {
                if (arr[j] > arr[j + 1]) {
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }
    }
}
class SelectionSort implements Sortable {
    public void sort(int[] arr) {
        int n = arr.length;
        for (int i = 0; i < n - 1; i++) {
            int minIndex = i;
            for (int j = i + 1; j < n; j++) {
                if (arr[j] < arr[minIndex]) {
                    minIndex = j;
                }
            }
            int temp = arr[minIndex];
            arr[minIndex] = arr[i];
            arr[i] = temp;
        }
    }
}
public class TestSort {
    public static void main(String[] args) {
        int[] arr1 = {5, 2, 9, 1, 6};
        Sortable ref;
        ref = new BubbleSort();
        ref.sort(arr1);
        System.out.println("Array sorted using BubbleSort:");
        for (int num : arr1) {
            System.out.print(num + " ");
        }
        System.out.println();
        int[] arr2 = {8, 3, 7, 4, 2};
        ref = new SelectionSort();
        ref.sort(arr2);
        System.out.println("Array sorted using SelectionSort:");
        for (int num : arr2) {
            System.out.print(num + " ");
        }
    }
}
```
# output
<img width="270" height="99" alt="5A" src="https://github.com/user-attachments/assets/82aa3371-a7a5-4fb0-beee-3c52306ab74f" />




# experiment5
## title:5b.)_runtime polymorphism
```
class Vehicle {
    void run() {
        System.out.println("Vehicle is running");
    }
}
class Car extends Vehicle {
    void run() {
        System.out.println("Car is running on four wheels");
    }
}
class Bike extends Vehicle {
    void run() {
        System.out.println("Bike is running on two wheels");
    }
}
public class TestVehicle {
    public static void main(String[] args) {
        Vehicle v;
        v = new Car();
        v.run();      
        v = new Bike();
        v.run();  
        v = new Vehicle();
        v.run();
}
}
```
# output
<img width="279" height="69" alt="5B" src="https://github.com/user-attachments/assets/c12a36da-2caa-487b-8a52-85a090f586ff" />


# experiment5
## title:5c.)string buffer to delete remove character
```
public class StringBufferDemo {
    public static void main(String[] args) {
        StringBuffer sb = new StringBuffer("Java Programming");     
        System.out.println("Original String: " + sb);
        sb.deleteCharAt(4);
        System.out.println("After deleting character at index 4: " + sb);
        sb.delete(0, 4);
        System.out.println("After deleting characters from index 0 to 4: " + sb);
    }
}
```
# output
<img width="434" height="63" alt="5c" src="https://github.com/user-attachments/assets/bb5ac1f1-d2f4-4c65-abe0-add07aa5ac92" />
