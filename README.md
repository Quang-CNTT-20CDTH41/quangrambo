package ontap;
import java.util.Scanner;
public class giaiphuongtrinhbac2 {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int a,b,c;
		System.out.printf("Nhap a: ");
		a = sc.nextInt();
		System.out.printf("Nhap b: ");
		b = sc.nextInt();
		System.out.printf("Nhap c: ");
		c = sc.nextInt();
		if(a==0) {
			if(b==0) {
				if(c==0) {
					System.out.printf("Phuong trinh vo so nghiem");
				}else {
					System.out.printf("Phuong trinh vo nghiem");
				}
			}else {
				System.out.printf("Phuong trinh co nghiem la: %d", (-b/c));
			}
		}else {
			double x1;
			double x2;
			double  delta = Math.pow(b, 2) - 4*a*c;
			if(delta<0) {
				System.out.printf("Phuong trinh vo nghiem");
			}else if(delta>0) {
				x1 = (-b+Math.sqrt(delta))/(2*a);
				x2 = (-b+Math.sqrt(delta))/(2*a);
				System.out.printf("Phuong trinh co nghiem x1 la: %f",x1);
				System.out.printf("Phuong trinh co nghiem x2 la: %f",x2);
			}else {
				System.out.printf("Phuong trinh co nghiem kep: %f",(-b)/2*a);
			}
		}
	}
}
