import java.util.Scanner;

public class Task03 {
    public static double balance = 0;

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Welcome! Please Enter:\n\"1\" To Deposit Amount\n\"2\" To Withdraw Amount\n\"3\" To Check Balance\n\"0\" To Exit");
        int choice = sc.nextInt();

        while(choice!=0){
            performOperation(choice);
            System.out.println("Welcome! Please Enter:\n\"1\" To Deposit Amount\n\"2\" To Withdraw Amount\n\"3\" To Check Balance\n\"0\" To Exit");
            choice = sc.nextInt();
        }

        System.out.println("Thank You For Using Our Services.");

        sc.close();
    }

    private static void performOperation(int choice) {
        Scanner sc = new Scanner(System.in);

        switch (choice) {
            case 1:
                System.out.print("Enter amount to deposit: ");
                double depositAmount = sc.nextDouble();
                balance += depositAmount;
                System.out.println("Deposit successful.\nCurrent Balance is: $" + balance);
                break;
            case 2:
                System.out.print("Enter the amount to withdraw: ");
                double withdrawalAmount = sc.nextDouble();
                if (withdrawalAmount > balance) {
                    System.out.println("Insufficient funds.");
                } else {
                    balance -= withdrawalAmount;
                    System.out.println("Withdrawal successful.\nCurrent Balance is: $" + balance);
                }
                break;
            case 3:
                System.out.println("Current balance is: $" + balance);
                break;
            case 0:
                break;
            default:
                System.out.println("Please enter a valid choice.");
        }
    }
}
