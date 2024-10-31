Print Parallelogram Star Pattern
In this program we’re going to code pyramid star pattern program .

In this program take a input from user and then store in the variable called as row and col then take for loop start from i=1 to i<=row and then take j inner for loop start from j=1 to j<=i  to print spaces then take another for loop to print statement star statement after that at the end of main outer loop take line change statement

Java Program for Parallelogram Star Pattern
Algorithm:
Take the number of rows and columns as input from the user ( length and breadth of the parallelogram) and store it in two different variables. (‘row’ and ‘col’ in this case)
Run a loop ‘row’ number of times to iterate through all the rows. From i=1 to i<=row. The loop should be structured as for (int i = 1; i <= row; i++)
 Run a nested loop ‘i’ times to print the spaces before the parallelogram. From j=0 to j<i. The loop should be structured as for (int j = 1; j <= i; j++).
Inside this nested loop print white sapce to print the trailing spaces before the parallelogram.
Run another nested loop ‘col’ times to iterate through each column of a row.
Inside this loop print star to print a start in each column of a row. for (int j = 1; j <= i; j++)
Inside the main loop move to the next line by printing a new line.  System.out.println();
Code in Java:
import java.util.Scanner;
public class Pattern1 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter row and col");
		int row = sc.nextInt();
		int col = sc.nextInt();
		
		for (int i = 1; i <= row; i++) {
			for (int j = 1; j <= i; j++) 
			    	System.out.print(" ");
			for (int j = 1; j <= col; j++) 
				System.out.print("*");
			System.out.println();
		}

	}

}
