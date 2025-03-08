# First-Assigment

import java.util.*;
public class Main {
    public static void main(String[] args) {
Scanner sc=new  Scanner (System.in);
        System.out.println("enter the number");
        int number = sc.nextInt();
        if(number <1 || number >99999){
            System.out.println("invalid number");
        }else {
            int a = number%10;
            int b= number/10;
            int c= b%10;
            int g= number /100;
            int d= g%10;
            int e= number /1000;

            String sD[]={"","one","two","three","four","five","six","seven","eight","nine","ten","eleven","twelve","thirten","fourteen","fifteen","sixteen","seventeen","eighteen","nineteen"};
            String ty[]={"","ten","twenty","thirty","fourty","fifty","sixty","seventy","eighty","ninety"};
            String h="hunderd";
            String th="thousand";
            if(number<20)
            System.out.println(sD[number]);
            else if(number>=20 && number<=100)
                System.out.println(ty[c]+" "+sD[a]);
            else if(number>=100 && number <999)
                System.out.println(sD[d]+" "+h+" "+ty[c]+" "+sD[a]);
            else
                System.out.println(sD[e]+" "+th+" "+sD[d]+" "+h+" "+ty[c]+" "+sD[a]);

        }
    }
}
