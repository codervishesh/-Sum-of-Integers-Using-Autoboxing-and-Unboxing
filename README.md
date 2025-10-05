# -Sum-of-Integers-Using-Autoboxing-and-Unboxing
 Sum of Integers Using Autoboxing and Unboxing Objective: To build a Java program that utilizes autoboxing and unboxing to calculate the sum of a list of integers. The program should also demonstrate parsing string inputs into integer values using methods like Integer.parseInt()
import java.util.ArrayList;
import java.util.Scanner;

public class SumUsingAutoboxing {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        ArrayList<Integer> numbers = new ArrayList<>();
        System.out.println("Enter integers separated by space:");
        String[] inputs = sc.nextLine().split(" ");
        for (String s : inputs) {
            numbers.add(Integer.parseInt(s));
        }
        int sum = 0;
        for (Integer num : numbers) {
            sum += num;
        }
        System.out.println("Total sum: " + sum);
    }
}
