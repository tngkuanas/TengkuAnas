package Week02;

/**
 *
 * @author tngku
 */
import java.util.Scanner;
public class L01Q02 {
    public static void main(String[] args){
        
        double P,D,R,Y,M;
        Scanner keyboard=new Scanner(System.in);
        System.out.println("Enter price of car");
        P = keyboard.nextDouble();
        System.out.println("Enter your down payment");
        D = keyboard.nextDouble();
        System.out.println("Enter interest rate in % ");
        R = keyboard.nextDouble();
        System.out.println("Enter loan duration in year");
        Y = keyboard.nextDouble();
        
        M=  (P - D) * (1 + R*Y/100) / (Y *12);
        
        System.out.printf("Your monthly payment is "+"%.2f%n",M);
        
        
        
    }
    
}

package Week02;

/**
 *
 * @author tngku
 */
import java.util.Scanner;
public class L02Q01 {
    public static void main(String[] args){
        double celcius,fahrenheit;
        Scanner keyboard = new Scanner(System.in);
        System.out.println("Enter the temperature in Fahrenheit");
        fahrenheit = keyboard.nextDouble();
        celcius = (fahrenheit - 32)/1.8;
        System.out.printf("Your temperature in celcius is %.2f%n",celcius);
        
    }   
}

package Week02;

/**
 *
 * @author tngku
 */
import java.util.Scanner;
public class L02Q04 {
    public static void main(String[] args){
        
        int time,hour,min,sec;
        
        Scanner keyboard = new Scanner(System.in);
        System.out.println("Enter your time in seconds");
        time = keyboard.nextInt();
        
        hour= time/3600;
        min = (time%3600)/60;
        sec =((time%3600)/60)%60;
        
        System.out.println(hour + " hours " + min + " minutes "+ sec + " Seconds ");
    }
    
}
