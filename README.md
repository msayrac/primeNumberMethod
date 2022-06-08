# primeNumberMethod

import java.util.Scanner;

public class Main {
    static int primeNum(int n){
        int count=0;
        for(int i=1;i<=n;i++){
            if(n%i==0){
                count++;
            }
        }
        if(count==2){
            System.out.println(n + " is a prime number");
        } else{

            System.out.println(n + " is NOT a prime number");
        }
        return 0;
    }
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.println("enter a number : ");
        int n = input.nextInt();

        primeNum(n);
    }
}
