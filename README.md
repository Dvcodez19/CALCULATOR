import java.util.Scanner;
public class d{
	public static void main(String[] args){
		Scanner sc = new Scanner(System.in);
		double a,b;
		System.out.print("Enter first number  : "); 
		a = sc.nextDouble();
		System.out.print("Enter second number  : "); 
		b = sc.nextDouble();
		char n;
		System.out.println("To perform addition press : +"); 
		System.out.println("To perform subtraction press : -"); 
	        System.out.println("To perform multiplication press : *"); 
		System.out.println("To perform division press : /"); 
		System.out.println("To perform remainder operation press : %"); 
		System.out.print("Enter which operation you want to perform : "); 
		n = sc.next().charAt(0);
		switch(n){
		case '+' :
		{
		System.out.println("Sum is  : "+(a+b)); 
		break;
		}
		case '-' :
		{
		System.out.println("Difference is  : "+(a-b)); 
		break;
		}
		case '*' :
		{
		System.out.println("Product is  : "+(a*b)); 
		break;
		}
		case '/' :
		{
		if(b!=0){
		System.out.println("Quotient is  : "+(a/b)); 
		break;
		}
		else{
		System.out.println("Cannot divide by zero");
		break;
		}
		}
		case '%' :
		{
		if(b!=0){
		System.out.println("Remainder is  : "+(a%b)); 
		break;
		}
		else{
		System.out.println("Cannot give remainder on dividing by zero"); 
		break;
		}
		}
		default:
		{
		System.out.print("Invalid Choice");
		break;
		}
		}
	}
}
