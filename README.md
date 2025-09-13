import java.util.Scanner;
public class SimpleCalculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("enter the first number: ");
        double num1 = sc.nextDouble();

        System.out.println("enter an operator(+,-,*,/): ");
        char operator = sc.next().charAt(0);

        System.out.println("enter second number: ");
        double num2= sc.nextDouble();

        double result;

        switch(operator){
            case '+':
            result= num1 + num2;
            System.out.println("result: " + result);
            break;
        

        case '-':
        result= num1-num2;
        System.out.println("result: "+ result);
        break;

        case '*':
        result = num1*num2;
        System.out.println("result: "+ result);
        break;

        case '/':
        if (num2 != 0) {
            result = num1 / num2;
            System.out.println("result: "+ result);
        }
        else{
            System.out.println("invalid can't be devided by 0");
        }
        break;

        default:
        System.out.println("invalid input");
        break;
    }


    sc.close();
        }
}
