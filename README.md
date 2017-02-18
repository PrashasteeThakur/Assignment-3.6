# Assignment-3.6

1.The method should be overloaded with the same return type in order to
avoid ambiguity.
For example,
class A{
static int add(int a,int b){return a+b;}
static double add(int a,int b){return a+b;}
}
class B{
public static void main(String[] args){
System.out.println(Adder.add(11,11));//ambiguity
}}
In this when code is compiled it will show error as:
Overloading3.java:3: error: method add(int,int) is already defined in class A
static double add(int a,int b){return a+b;}

To overcome this problem method should be overloaded with the same return type.


8.
import java.util.*;
public class acad{
public static void main(String[] args){
Scanner sc=new Scanner(System.in);
int n=sc.nextInt();   //size of array
int[] a=new int[n];
for(int i=0;i<n;i++)
{
a[i]=sc.nextInt();
}
Arrays.sort(a);   //sorting array
for(int i=a.length-1;;i>=0;i--){
System.out.println(a[i]+" ");  //displaying sorted reversed order array elements
}
}
}
