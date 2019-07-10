import java.util.Scanner;

public class Plane {
	public static void main(String[] args) {
	Scanner input = new Scanner(System.in);	
	
	boolean[] seats = new boolean[10]; //array of seats
	int firstClass = 0; //next available first class seat
	int economy = 5; //next avail economy seat
	
	while ((firstClass < 5) || (economy < 10)) {
		System.out.println("Please type 1 for First Class");
		System.out.println("Please type 2 for Economy");
		System.out.print("Choice: ");
		int section = input.nextInt();
		
		if (section == 1) {
			if (firstClass < 5) {
				firstClass++;
				System.out.printf("First Class. Seat #%d\n", firstClass);
			}
			else if (economy < 10) {//first class full
				System.out.println("First Class is full, would you like Economy Class instead?");
				System.out.print("1. Yes, 2. No. Your choice: ");
				int choice = input.nextInt();
				if (choice == 1) {
					economy++;
					System.out.printf("Economy Class. Seat #%d\n", economy);
				}
				else {
					System.out.println("Next flight leaves in 3 hours.");
				}
			}
		}
		else if (section == 2) {
			if (economy < 10) {
				economy++;
				System.out.printf("Economy Class. Seat #%d\n", economy);
			}
			else if (firstClass < 5) {
				//economy is full
			System.out.println("Economy Class is full, would you like First Class instead?");
			System.out.print("1. Yes, 2. No. Your choice: ");
			int choice = input.nextInt();
			
			if (choice == 1) {
				firstClass++;
				System.out.printf("First Class. Seat #%d\n", firstClass);
			}
			else {
				System.out.println("Next flight leaves in 3 hours.");
			}
			}
		}
	System.out.println();
	
	}
		System.out.println("The plane is now full.");
	}	
}
