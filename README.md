# 210111
package basic;

import java.util.Scanner;

public class CodeUp1567 {

	static int n,m;
	static long[] prefix;
	static long[] arr;
	public static void main(String[] args) {
		// TODO Auto-generated method stub
		f();
	}
	static void f() {
		Scanner sc=new Scanner(System.in);
		 n=sc.nextInt();
		 prefix=new long[n+2];
		 arr=new long[n+1];
		 for (int i = 0; i < n; i++) {
			 arr[i]=sc.nextLong();
		 }
		 int s=sc.nextInt();
		 int e=sc.nextInt();
		 
		 int res=0;
		 for (int i = s; i <= e; i++) {	
			  res+=arr[i-1];
		}
		 System.out.print(res+" ");
		
	}
}
