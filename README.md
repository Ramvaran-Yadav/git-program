import java.util.Scanner;

public class lcm {


    static void main() {
        Scanner Sc=new Scanner(System.in);
        System.out.println("Enter The two number that You Find The LCM:: ");
        int input1=Sc.nextInt();
        int input2=Sc.nextInt();
        int lcm=lcm(input1,input2);
        System.out.println(lcm);
    }



    public static int lcm(int num1,int num2){
        System.out.println("Your First Number:: "+num1);
        System.out.println("Your Second Number:: "+num2);
        int i=1;
        int fact;
        while (i<=num2){
            fact=num1*i;
            if (fact%num2==0){
                return fact;
            }
            i++;
        }
        return 0;


    }
}
