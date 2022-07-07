# Palindrome-Using-Java
To find whether the number is palindrome or not

package Pp;

import java.util.Scanner;

public class palindrome {

	public static void main(String[] args){
		
		Scanner sc = new Scanner(System.in);
		
		System.out.println("Enter a number:");
		
		int number = sc.nextInt();
		int real;
		int ans = 0;
		int temp;

		
		temp = number ;
		
		while(number > 0) {
			real = number % 10;
			
			ans = (ans * 10) + real;
			
			number = number / 10;
		}
		
		if(temp == ans) {
			
			System.out.println(temp + " is a palindrome number");
			
		}
		
		else {
			
			System.out.println(temp + "is not a palindrome number");
			
		}

			
	}
	
}
