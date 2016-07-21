# CheckSumOfDigitIsPalindrome
import java.util.Scanner;

public class CheckSumIsPalindrome {

	
	public static void main(String[] args) {
		
		Scanner input = new Scanner(System.in);
		System.out.println("Enter number");
		int get=input.nextInt();
		int sum=0;
		int sum1=0;
		int dumy=get;
		while(dumy!=0)
		{
			sum=sum+(dumy%10);
			dumy=dumy/10;
		}
		int opsum=sum;
		while(opsum!=0){
			sum1=sum1*10;
			sum1=sum1+(opsum%10);
			opsum=opsum/10;
		}
		if(sum==sum1)
		{
			System.out.println("Sum of digit is palindrome");
		}
		else{
			System.out.println("It is not a palindrome");
		}

	}

}
