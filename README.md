import java.util.Scanner;

class Armstrong{

    public static void main(String[] args) {

        int a, digit, cube = 0,num;
        
        System.out.println("Enter the number:");
        Scanner sc = new Scanner(System. in );
        num = sc.nextInt();
        a = num;

        while (num!= 0)
        {
            digit = num % 10;
            cube+= Math.pow(digit, 3);
            num =num/10;
        }

        if(cube == a)
            System.out.println(a+ " is a Armstrong number");
        else
            System.out.println(a+ " is not a Armstrong number");
    }
}
