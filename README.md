import java.util.Scanner;
public class b {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
            int computerNumber=(int)(Math.random()*10)+1;
            int userGuess;
            int count=0;
            do{
                System.out.println("Guess the number 1 and 10");
                userGuess= sc.nextInt();
                if (userGuess>computerNumber){
                    System.out.println("too high,try again");
                } else if (userGuess<computerNumber) {
                    System.out.println("too low,try again");
                }else{
                    System.out.println("You have guessed correct number");
                    System.out.println("and it was 0" +userGuess);
                    count++;
                    System.out.println("chance"+count+"done and"+"remaining chance is "+(3-count));
                }
            }
            while (true&&count<3);
        }
    }# Number-Gussing
