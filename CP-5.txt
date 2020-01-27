
import java.util.Scanner;

/**
 *
 * @author Masum Khan
 */
class Dick {

    public static void main(String[] args) {

        Scanner scn = new Scanner(System.in);

        int n1, n2, n3;
        while (scn.hasNext()) {
            n1 = scn.nextInt();
            n2 = scn.nextInt();
            n3 = scn.nextInt();
            if (n1 > n2 && n1 > n3) {
                if (n2 > n3) {
                    n1 = n2;

                } else {
                    n1 = n3;
                }

            }
            if (n2 > n1 && n2 > n3) {
                if (n1 > n3) {
                    n2 = n1;
                } else {
                    n2 = n3;
                }

            }
            if (n3 > n1 && n3 > n2) {
                if (n1 > n2) {
                    n3 = n1;
                } else {
                    n3 = n2;
                }
            }
            System.out.println(n1 + n2 + n3);
        }
    }
}
