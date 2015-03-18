import java.util.Scanner;

public class Lab2Week6 {
	public static void main(String[] args) {

		Scanner keyboard = new Scanner(System.in);

		int guess;
		int secretNumber;

		int count = 1;
		while (count < 4) {
			count++;
			
			System.out.print("Enter a guess: ");
			secretNumber = (int) (Math.random() * 10 + 0);
			guess = keyboard.nextInt();
			System.out.println("Your guess is " + guess);

			if (guess < secretNumber) {
				System.out
						.println("Your guess is smaller than the secret number."
								+ secretNumber);
			} else if (guess > secretNumber) {
				System.out
						.println("Your guess is greater than the secret number."
								+ secretNumber);
			} else if (guess == secretNumber) {
				System.out.println("Your guess is correct. Congratulations!"
						+ secretNumber);
			
					
				}
			
			
			}
		
		System.out.println("Bye");
			
			

		}
		
	}

