
import java.util.Scanner;

class Valid {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter code: ");
        String code = sc.nextLine();

        String rev = "";
        for (int i = code.length() - 1; i >= 0; i--) {
            rev = rev + code.charAt(i);
        }

        if (code.equals(rev)) {
            System.out.println("Security code is valid");
        } else {
            System.out.println("Security code is invalid");
        }
    }
}
