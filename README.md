import java.util.Scanner;
class Eb
{
	public static void main(String []args)
	{
		Scanner sc=new Scanner(System.in);
		System.out.println("Enter the units consumed in (kwh)");
		double units=sc.nextFloat();
		double bill=0;
		if(units<=100)
		{
			bill=units*0;
		}
		else if(units>100 && units<=200)
		{
			bill=(units-100)*2.25;
		}
		else if(units>200 && units<=400) {
			bill=(100*2.25)+(units-200)*4.50;
		}
		else if(units>400 && units<=500) {
			bill=(100*2.25)+(200*4)+(units-400)*5.00;
		}
		else if(units>600 && units<=700) {
			bill=(100*2.25)+(200*4)+(400*5)+(units-600)*6.00;
		}
		else if(units>700 && units<=800) {
			bill=(100*2.25)+(200*4)+(400*5)+(700*6)+(units-700)*8.00;
		}
		else if(units>800 && units<=900) {
			bill=(100*2.25)+(200*4)+(400*5)+(700*6)+(800*8)+(units-800)*9.00;
			}
		else if(units>900 && units<=1000) {
			bill=(100*2.25)+(200*4)+(400*5)+(700*6)+(800*8)+(900*9)+(units-900)*10.00;	
		}
		else if(units>=1000) {
			bill=(units)*11.00;
		}
		System.out.println("Bill to pay is ="+bill);
	}
