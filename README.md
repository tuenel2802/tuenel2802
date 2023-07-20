
import java.util.Scanner;

public class Practicejj {
	public static void taoMang(double arr[], int n) {
		Scanner input= new Scanner(System.in);
		for (int i=0;i<n;i++)
		{
			arr[i] = input.nextDouble();
		}
	}
	
	public static void inMang(double arr[], int n) {
		for (int i=0;i<n;i++)
		{
			System.out.printf(arr[i] + " ");
		}
	}
	
	public static double timMax (double arr[], int n) {
		double max = arr[0];
		for (int i=0;i<n;i++)
		{
			if (max < arr[i])
				max = arr[i];
		}
		return max;
	}
	
	public static double timMin (double arr[], int n) {
		double min = arr[0];
		for (int i=0;i<n;i++)
		{
			if (min > arr[i])
				min = arr[i];
		}
		return min;
	}
	
	public static void main(String[] args) {
		Scanner input= new Scanner(System.in);
		int a = input.nextInt();
		double arr[] = new double[a];
		taoMang(arr,a);
		System.out.println("Max = " + timMax(arr,a));
		System.out.println("Min = " + timMin(arr,a));
	}

}
