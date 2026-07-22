
package javaapplication2;
import java.util.Scanner;
public class JavaApplication2 
{
     int cno,pre_re,cur_re;
     int unit;
     String type;
     String name;
     double amount; 
     void input()
     {
         Scanner in=new Scanner(System.in);
         System.out.println("Enter Consumer Name");
         name=in.next();
         System.out.println("Enter Previous meter reading ");
         pre_re=in.nextInt();
         System.out.println("Enter Current meter reading ");
         cur_re=in.nextInt();
         System.out.println("Enter the Type");
         type=in.next();
         
     }
     void Amount()
     {
         unit=cur_re-pre_re;
         if (type.equals("Domestic"))
                 {
                     if (unit<=100)
                     {
                         amount=0;
                     }
                     else if (unit<=200)
                             {
                                 amount=(unit-100 )*2;
                             }
                     else if (unit<=500) 
                         {
                         amount=(100*2)+(unit-200)*4;
                         }
                     else 
                     {
                         amount=(100*2)+(300*4)+(unit-500)*6;
                     }
                     
                  }
         else if (type.equals("Commerical"))
                 {
                     if (unit<=100)
                     {
                         amount=unit*2;
                     }
                     else if (unit<=200)
                             {
                                 amount=(100*2)+(unit-100)*4;
                             }
                     else if (unit<=500) 
                         {
                             amount=(100*2)+(300*4)+(unit-200)*6;
                         }
                     else 
                     {
                         amount=(100*2)+(300*4)+(500*6)+(unit-500)*7;
                     }
                     
                  }
         
                 }
     void output()
     {
         System.out.println("......EB Bill.......");
         System.out.println("Consumer Name      :"+name);
         System.out.println("Connection Type    :" +type);
         System.out.println("Unit consumed      :" +unit);
         System.out.println("Amount to be paid  :" +amount);
     }
     

             
    public static void main(String[] args) 
    { 
       JavaApplication2 in=new JavaApplication2();
       in.input();
       in.Amount();
       in.output();
    }
    
}
