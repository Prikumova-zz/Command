# Command
import java.util.Scanner;

public class CommonDivaisors {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		System.out.println("Insert the number");
		Scanner in = new Scanner (System.in);
		int n = in.nextInt();
		int [] arr1 = new int [n];
		int [] arr2 = new int [n];
		int [] arr3 = new int [n];
		for(int i = 0; i<2*n; i++) {
			if (i<n) {
				arr1[i]=in.nextInt();
			}
			else {
				arr2[i-n]=in.nextInt();
			}
		}
		for (int i=0; i<n; i++) {
			if (arr1[i]>arr2[i]) {
				arr3[i]=arr1[i];}
				else {
					arr3[i]=arr2[i];
				
			}
		}
	}	
}
