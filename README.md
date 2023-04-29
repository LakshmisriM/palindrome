# palindrome
import java.util.Scanner;
class palindrome
{
    public static void main(String args[])
    {
        int temp,remainder,sum=0;
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter a value:");
        int number=sc.nextInt();
        temp=number;
        while(number>0)
        {
            remainder=number%10;
            sum=sum*10+remainder;
            number=number/10;
        }
        if(temp==sum)
        {
            System.out.println("The Given Number is Palindrome");
        }
        else
        {
            System.out.println("The Given Number Not a Palindrome");
        }
    }
}
