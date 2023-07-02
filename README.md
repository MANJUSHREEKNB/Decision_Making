//Electricity Bill
//JAVA CODE
import java.io.*;
import java.util.*;
public class Solution {
    public static void main(String[] args) {
        Scanner sc=new Scanner (System.in);
        int unit=sc.nextInt();
        if (unit<=200){
            float pay=(unit*0.5f);
            System.out.println("Rs."+(int)pay);
        }
        else if(unit<=400){
            float pay=(unit*0.65f)+100;
            System.out.println("Rs."+(int)pay);
        }
        else if(unit<=600){
            float pay=(unit*0.80f)+200;
            System.out.println("Rs."+(int)pay);
        }
        else if (unit>600){
            float pay=(unit*1.25f)+425;
            System.out.println("Rs."+(int)pay);
        }
    }
}

//TRENDY NUMBER
//JAVA CODE
import java.io.*;
import java.util.*;
public class Solution {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int num=sc.nextInt();
        if ((num<=999)&&(num>=100)){
            int var=(num/10)%10;
            if (var%3==0){
                System.out.println("Trendy Number");
            } 
            else
            System.out.println("Not a Trendy Number");
            }
        else
            System.out.println("Invalid Number");
    }
}

//TIME SHEET
//JAVA CODE
import java.io.*;
import java.util.*;
public class Solution {
    public static void main(String[] args) {
        Scanner sc=new Scanner (System.in);
        int d1=sc.nextInt();
        int d2=sc.nextInt();
        int d3=sc.nextInt();
        int d4=sc.nextInt();
        int d5=sc.nextInt();
        int d6=sc.nextInt();
        int d7=sc.nextInt();
        int sum=0;
        sum+=d1*150;
        sum+=d7*125;
        if (d2<=8){
            sum+=d2*100;
        }
        else{
            sum+=(d2-8)*115+800;
        }
        if (d3<=8){
            sum+=d3*100;
        }
        else{
            sum+=(d3-8)*115+800;
        }
        if (d4<=8){
            sum+=d4*100;
        }
        else{
            sum+=(d4-8)*115+800;
        }
        if (d5<=8){
            sum+=d5*100;
        }
        else{
            sum+=(d5-8)*115+800;
        }
        if (d6<=8){
            sum+=d6*100;
        }
        else{
            sum+=(d6-8)*115+800;
        }
        System.out.println(sum);
    }
}
