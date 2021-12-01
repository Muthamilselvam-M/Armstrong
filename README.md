# Armstrong




import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
       // Scanner in = new Scanner(System.in);
        ///System.out.print("Enter an Integer:");
        //int a=in.nextInt();
        for (int i=2;i<=1000;i++) {
            if (armStrong(i)!=0)
            System.out.println(armStrong(i));
        }

    }
    public static int armStrong(int num){
        int x,y,z=0;
        int num1 = num;
        while(num>0){
             x = num%10;
             y = x * x * x;
             z += y;
             num = num/10;



        }
        if (num1==z)
      return z;
        else{
            return 0;
        }
    }
}
