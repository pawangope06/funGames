# FUN GAMES USING JAVA
# this game is guessing the number of programmer by user in given limit

import java.util.Scanner;

public class GuessAnumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        /*
        this program is on guessing the secret number of a programmer
        the secret number is given by the programmer
        and the user has to guess the number within the given limit
         */
        int secret_number = 7;
        int limit = 3;
        System.out.println("YOU HAVE "+limit+" CHANCES");
        for (int i=1; i<=limit; i++){
            System.out.println("ENTER NUMBER "+i);
            int guess_number = sc.nextInt();
            if (guess_number == secret_number){
                System.out.println("HURRAY");
                break;
            }
            else
                System.out.println("OOPS, WRONG GUESS");
        }
        System.out.println("\nDO YOU WANT TO RE-PLAY THIS GAME");
        System.out.println("IF YES PRESS 1");
        System.out.println("IF NO PRESS 0");
        int check = sc.nextInt();
        if (check == 1){
            for (int i=1; i<=limit; i++){
                System.out.println("ENTER NUMBER "+i);
                int guess_number = sc.nextInt();
                if (guess_number == secret_number){
                    System.out.println("HURRAY");
                    break;
                }
                else
                    System.out.println("OOPS, WRONG GUESS");

            }

        } else if (check == 0) {
            System.out.println("SEE YOU AGAIN");
        }
        System.out.println("RE-START");
    }
}
