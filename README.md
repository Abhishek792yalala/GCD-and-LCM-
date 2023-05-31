# GCD-and-LCM-

GCD & LCM

import java.util.*;

class GCDLCM{

    static void LCM(int a, int b){

        int lcm; int prod; int i=1;

        lcm=prod=a*b;

        System.out.println("Least Common Multiple of a and b is: "+ lcm);

    }

    public static void main(String... args){

        System.out.println("Enter the value of a and b: ");

        Scanner sc=new Scanner(System.in);

        int a=sc.nextInt();

        int b=sc.nextInt();

        int min=0;

        if(a>b){

            min=b;

        }

        if(b>a){

            min=a;

        }

        for(int i=min;i>=1;i--){

            if((a%i==0) && (b%i==0)){

                System.out.println("The Greatest Common Divisor of a and b is : "+ i);

                break;

            }

        }

        LCM(a,b);

    }

}

/*

Enter the value of a and b:

5

10

The Greatest Common Divisor of a and b is : 5

Least Common Multiple of a and b is: 50

***********************************************

2

3

The Greatest Common Divisor of a and b is : 1

Least Common Multiple of a and b is: 6

 */
